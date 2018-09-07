# Bellman-Ford
Dijkstra’s Algorithm doesn’t work for Graphs with negative weight edges, whilst Bellman-Ford works for such graphs. On the other hand, time complexity of Bellman-Ford is O(VE), which is more than Dijkstra.

The Bellman–Ford algorithm finds shortest paths from a starting node to all nodes of the graph. The algorithm can process all kinds of graphs, provided that the graph does not contain a cycle with negative length. If the graph contains a negative cycle, the algorithm can detect this. Like other Dynamic Programming Problems, the algorithm calculate shortest paths in bottom-up manner. It first calculates the shortest distances which have at-most one edge in the path. Then, it calculates shortest paths with at-most 2 edges, and so on. After the i-th iteration of outer loop, the shortest paths with at most i edges are calculated. 
The algorithm keeps track of distances from the starting node to all nodes of the graph. Initially, the distance to the starting node is 0 and the distance to any other node is infinite. The algorithm then reduces the distances by finding edges that shorten the paths until it is not possible to reduce any distance.
 <p align="center">
  <img width="430" height="320" src="https://user-images.githubusercontent.com/35730663/45238793-a8244800-b2a8-11e8-8c85-c722d42d30dd.png">
</p>
