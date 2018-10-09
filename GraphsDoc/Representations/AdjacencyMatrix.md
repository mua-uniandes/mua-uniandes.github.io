# Adjacency Matrix

An *adjacency matrix* indicates the edges that a graph contains. We can efficiently check from an adjacency matrix if there is an edge between two nodes. The matrix can be stored as an array where each value adj[a][b] indicates whether the graph contains an edge from node a to node b. If the edge is included in the graph, then adj[a][b] = 1, and otherwise  adj[a][b] = 0.

The drawback of the adjacency matrix representation is that an adjacency matrix contains n2 elements, and usually most of them are zero. For this reason, the representation cannot be used if the graph is large.

```
int n;
boolean [][] a;
AdjacencyMatrix (int si){
n = si;
a = new boolean[n][n];
}


    void addEdge(int i, int j) {
        a[i][j] = true;
    }
    void removeEdge(int i, int j) {
        a[i][j] = false;
    }
    boolean hasEdge(int i, int j) {
        return a[i][j];
    }
```
 <p align="center">
  <img width="260" height="320" src="https://user-images.githubusercontent.com/35730663/45234509-91c3bf80-b29b-11e8-9458-6c42d6b49c3b.png">
</p>

[Java Implementation](https://github.com/mua-uniandes/weekly-problems/blob/master/Implementations/Java/Graphs-AdjacencyMatrix.java)
