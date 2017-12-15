# Homework 11

1. Exercises 24.4-2<br>
Find a feasible solution or determine that no feasible solution exists for the following system of difference constraints:

    x<sub>1</sub> - x<sub>2</sub> ≤ 4,
    x<sub>1</sub> - x<sub>5</sub> ≤ 5,
    x<sub>2</sub> - x<sub>4</sub> ≤ -6,
    x<sub>3</sub> - x<sub>2</sub> ≤ 1,
    x<sub>4</sub> - x<sub>1</sub> ≤ 3,
    x<sub>4</sub> - x<sub>3</sub> ≤ 5,
    x<sub>4</sub> - x<sub>5</sub> ≤ 10,
    x<sub>5</sub> - x<sub>3</sub> ≤ -4,
    x<sub>5</sub> - x<sub>4</sub> ≤ -8.

2. Problem 24-3 Arbitrage<br>
**Arbitrage** is the use of discrepancies in currency exchange rates to transform one unit of a currency into more than one unit of the same currency. For example, suppose that 1 U.S. dollar buys 49 Indian rupees, 1 Indian rupee buys 2 Japanese yen, and 1 Japanese yen buys 0.0107 U.S. dollars. Then, by converting currencies, a trader can start with 1 U.S. dollar and buy 49 × 2 × 0.0107 = 1.0486 U.S. dollars, thus turning a profit of 4.86 percent.<br>
Suppose that we are given n currencies c<sub>1</sub>, c<sub>2</sub>, … , c<sub>n</sub> and an n × n table R of exchange rates, such that one unit of currency c<sub>i</sub> buys R[i, j] units of currency c<sub>j</sub>.
    - Give an efficient algorithm to determine whether or not there exists a sequence of currencies [ c<sub>i<sub>1</sub></sub>, c<sub>i<sub>2</sub></sub>, … , c<sub>i<sub>k</sub></sub> ] such that
R[i<sub>1</sub>, i<sub>2</sub>] ⋅ R[i<sub>2</sub>, i<sub>3</sub>] ⋅⋅⋅ R[i<sub>k-1</sub>, i<sub>k</sub>] ⋅ R[i<sub>k</sub>, i<sub>1</sub>] > 1 .
Analyze the running time of your algorithm.
    - Give an efficient algorithm to print out such a sequence if one exists. Analyze the running time of your algorithm.

3. Exercises 25.1-10<br>
Give an efficient algorithm to find the length (number of edges) of a minimum-length negative-weight cycle in a graph.

4. Show whether the Floyd-Warshall algorithm can detect negative-weight cycles. If yes, show how to find one of them.
    - **constructing...**

5. Exercises 25.2-1<br>
Run the Floyd-Warshall algorithm on the weighted, directed graph of figure below. and answer the following questions:
    - Show the matrix d<sup>(k)</sup> that results for each iteration of the outer loop.
    - List the vertices of one such shortest path from v<sub>6</sub> to v<sub>1</sub>.

![p5_figure](https://i.imgur.com/R3Mx8lq.png)

6. Exercises 25.3-1<br>
Use Johnson's algorithm to find the shortest paths between all pairs of vertices in the graph of figure below. Show the values of h and w' computed by the algorithm.

![p6_figure](https://i.imgur.com/R3Mx8lq.png)

7. Problem 25-1: Transitive closure of a dynamic graph<br>
Suppose that we wish to maintain the transitive closure of a directed graph G = (V, E) as we insert edges into E. That is, after each edge has been inserted, we want to update the transitive closure of the edges inserted so far. Assume that the graph G has no edges initially and that we represent the transitive closure as a Boolean matrix.
    - Show how to update the transitive closure G<sup>\*</sup>= (V, E<sup>\*</sup>) of a graph G = (V, E) in O(V<sup>2</sup>) time when a new edge is added to G.
    - Give an example of a graph G and an edge e such that O(V<sup>2</sup>) time is required to update the transitive closure after the insertion of e into G, no matter what algorithm is used.
    - Describe an efficient algorithm for updating the transitive closure as edges are inserted into the graph. For any sequence of n insertions, your algorithm should run in total time ![sum(t_i)=O(V^3)](http://latex.codecogs.com/gif.latex?%5CSigma_%7Bi%3D1%7D%5Ent_i%3DO%28V%5E3%29) , where t<sub>i</sub> is the time to update the transitive closure upon inserting the ith edge. Prove that your algorithm attains this time bound. 
