# Description
This algorithm can be used for processing large graphs. However, the algorithm requires that there are **no negative weight edges** in the graph. Dijkstra’s algorithm maintains distances to the nodes and reduces them during the search. At each step, Dijkstra’s algorithm selects a node that has not been processed yet and whose distance is as small as possible. Then, the algorithm goes through all edges that start at the node and reduces the distances using them. Dijkstra’s algorithm is efficient, because it only processes each edge in the graph once, using the fact that there are no negative edges. 
We generate a SPT ,shortest path tree, with given source (a graph and a source vertex in the graph) as root. We maintain two sets, one set contains vertices included in shortest path tree, and other set includes vertices not yet included in shortest path tree. At every step of the algorithm, we find a vertex which is in the other set (set of not yet included) and has a minimum distance from the source.
The algorithm processes the nodes in the order 1, 5, 4, 2, 3, and at each node reduces distances using edges that start at the node. Note that the distance to a node never changes after processing the node.+


 <p align="center">
  <img width="400" height="490" src="https://user-images.githubusercontent.com/35730663/45238553-d190a400-b2a7-11e8-9561-5d1fd406e509.png">
</p>


An efficient implementation of Dijkstra’s algorithm requires that we can efficiently find the minimum-distance node that has not been processed. An appropriate data structure for this is a priority queue that contains the remaining nodes ordered by their distances. Dijksra’s algorithm is a ***Greedy algorithm*** and time complexity is O(VLogV) (with the use of Fibonacci heap).
