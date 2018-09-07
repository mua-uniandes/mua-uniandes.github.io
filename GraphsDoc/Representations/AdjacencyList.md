# Adjacency List

 In the adjacency list representation, each node x of the graph is assigned an adjacency list that consists of nodes to which there is an edge from x. Adjacency lists are the most popular way to represent graphs, and most algorithms can be efficiently implemented using them. 
 
 A convenient way to store the adjacency lists is to declare an array of vectors. 
 
 ```
 vector <int> adj[N];
 adj[1].push_back(2);
 adj[2].push_back(3);
 adj[2].push_back(4);
 adj[3].push_back(4);
 adj[4].push_back(1);
 ```
   <p align="center">
  <img width="220" height="160" src="https://user-images.githubusercontent.com/35730663/45233890-ca629980-b299-11e8-9bbc-2107350400d6.png">
  </p>
