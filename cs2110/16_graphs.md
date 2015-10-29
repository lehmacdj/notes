# Graphs
+ A collection of elements which consists of nodes and edges
+ Biparteid -- graph with two separate regions
+ Directed graph (diagraph) -- graph with arrows to represent direction, uses ordered pairs
+ Undirected graph - like directed graph except unordered pairs are used
+ Complete graph (K\_n) -- a graph where there is a connection between any two nodes
+ Orientation of nodes does not matter

## Nodes
+ a collection of points 
+ denoted V
+ called source and sink in an directed graph
+ endpoints of the ordered pair

## Edges
+ a connection between two nodes denoted by pairs of points
+ Denoted by E

## Adjacency
+ when two nodes are connected by the edge

## Neighborhood
+ points that are adjacent to a certain node

## Degree
+ The number of nodes adjacent to a certain node

### Outdegree
+ number of edges for which a vertex is the source

### Indegree
+ number of edges for which a vertex is the sink

## Path
+ a sequence of vertices such that there is a connection between those two paths

### Length of a path
+ the number of edges in a path

### Simple
+ a path is simple if it doesn't repeat any vertices

### Cycle
+ where the start and end node are the same
+ a cycle is simple if no vertices are repeated except for the first and last
+ acyclic means that there are no cycles
+ A directed acyclic graph is a DAG
    + this can be determined by deleting indegree-0 vertices until the graph disappears ( or doesn't: then it has a cycle )

## Topological sort
+ an ordering of a graph where no vertex later in the list leads to a node earlier in the list

## Coloring
+ an assignment of a color to each node such that no two adjacent vertices get the same color
+ the question is how many colors are needed to complete the graph

## Planarity
+ If a graph can be drawn without any edges crossing

### Kuratowski's Theorem
+ a graph is planar if and only if it does not contain a copy of K5 or K3,3
+ possibly with other nodes along the edges of K5 or K3,3

### Four-Color Theorem
+ every planar graph is 4-colorable
+ a computer was used to do the proof

### Bipartide
+ always two colorable

## Data Structures
+ How do we represent graphs?

### Adjacency List
+ A list is kept for every node
+ the list contains the outgoing edges from that node
+ uses O(m + n) space
+ can iterate over all edges in time O(m + n)
+ Can answer "is there an edge from u to v?" in O(d(u)) time
+ better for sparse graphs

### Adjacency Matrix
+ A 2D matrix with 2 indexes for each node
+ Uses O(n^2) space
+ can iterate over all edges in O(n^2)
+ checking "is there an edge from u to v?" is O(1)
+ better for dense graphs

## Algorithms
### Search
+ how do we visit each node without too much additional data

#### Depth first 
+ Searches first along the deepest way to go
+ we keep an array of each of the nodes that has already been visited
+ a node is reachable if there is a path to that node for which all nodes in the path are unvisited
    + from a node which has been visited there are no REACHABLE nodes because it itself has already been visited

```java
/** Node u is unvisited. Visit all nodes that are REACHABLE from u. */
public static void dfs(int u) {
    visited[u] = true;
    for all edges (u, v) leaving u:
        if v is unvisited then dfs(v);
}
```

+ Suppose n nodes are reachable along m edges
    + O(n + m) run time
    + O(n + m) space usage

#### Breadth first
+ searches first based on distance from the initial node
+ same as depth first except Stack is replaced with a Queue
