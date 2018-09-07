# Description
Breadth First Search—abbreviated as BFS—is another graph traversal algorithm. Starting from a distinguished source vertex, BFS will traverse the graph ‘breadth-first’. That is, BFS will visit vertices that are direct neighbors of the source vertex (first layer), neighbors of direct neighbors (second layer), and so on, layer by layer. BFS starts with the insertion of the source vertex s into a queue, then processes the queue as follows: Take out the front most vertex u from the queue, enqueue all unvisited neighbors of u (usually, the neighbors are ordered based on their vertex numbers), and mark them as visited.

<p align="center">
  <img width="360" height="290" src="https://user-images.githubusercontent.com/35730663/45238309-10722a00-b2a7-11e8-80b7-7a161583f7f0.png">
</p>



With the help of the queue, BFS will visit vertex s and all vertices in the connected component that contains s layer by layer. BFS algorithm also runs in O (V +E) and O (V 2) on a graph represented using an Adjacency List and Adjacency Matrix, respectively.
