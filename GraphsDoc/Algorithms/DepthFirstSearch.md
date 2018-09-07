# Description

Depth First Search—abbreviated as DFS—is a simple algorithm for traversing a graph. Starting from a distinguished source vertex, DFS will traverse the graph ‘depth-first’. Every time DFS hits a branching point (a vertex with more than one neighbors), DFS will choose one of the unvisited neighbor(s) and visit this neighbor vertex. DFS repeats this process and goes deeper until it reaches a vertex where it cannot go any deeper. When this happens, DFS will ‘backtrack’ and explore another unvisited neighbor(s), if any.



 <p align="center">
  <img width="300" height="450" src="https://user-images.githubusercontent.com/35730663/45238080-35b26880-b2a6-11e8-8e70-65fec670793d.png">
</p>

 <p align="center">
  <img width="590" height="720" src="https://user-images.githubusercontent.com/35730663/45238092-419e2a80-b2a6-11e8-98d4-f747cc94203c.png">
</p>





The time complexity of this DFS implementation depends on the graph data structure used. In a graph with V vertices and E edges, DFS runs in O (V + E) and O (V 2) if the graph is stored as Adjacency List and Adjacency Matrix, respectively.
