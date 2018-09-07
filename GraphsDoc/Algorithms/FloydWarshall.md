# Floyd-Warshall
The Floyd–Warshall algorithm provides an alternative way to approach the problem of finding shortest paths. Unlike the other algorithms, it **finds shortest paths between all node pairs of the graph in a single run**.

The algorithm maintains a matrix that contains distances between the nodes. The initial matrix is directly constructed based on the adjacency matrix of the graph. Then, the algorithm consists of consecutive rounds, and on each round, it selects a new node that can act as an intermediate node in paths from now on, and reduces distances using this node.
 <p align="center">
  <img width="200" height="110" src="https://user-images.githubusercontent.com/35730663/45238802-ae1a2900-b2a8-11e8-95f7-2d56981dd7cd.png">
</p>
The idea is to one by one pick all vertices and updates all shortest paths which include the picked vertex as an intermediate vertex in the shortest path. When we pick vertex number k as an intermediate vertex, we already have considered vertices {0, 1, 2, .. k-1} as intermediate vertices. For every pair (i, j) of the source and destination vertices respectively, there are two possible cases.
