# Description
An *edge list* contains all edges of a graph in some order. This is a convenient way to represent a graph if the algorithm processes all its edges, and it is not needed to find edges that start at a given node. Each element in this list is of the form (a, b,w), which means that there is an edge from node a to node b with weight w.

. To represent an edge, we just have an array of two vertex numbers, or an array of objects containing the vertex numbers of the vertices that the edges are incident on. If edges have weights, add either a third element to the array or more information to the object, giving the edge's weight. Since each edge contains just two or three numbers, the total space for an edge list is  Θ(E).
```
[[1,2], [2,0], [5,8], [8,0]] 
```
