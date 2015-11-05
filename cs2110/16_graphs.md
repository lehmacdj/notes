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

## Shortest paths
+ Settled set -- shortest path to node is known
+ Frontier set -- shortest path is not yet known

### Precondition
1. The nodes in a graph are numbered 0..n-1
2. each edge has a positive weight
3. weight(v1, v2) is the weight of the edge from node v1 to v2
4. some node v is the start node
5. calculate the length of shortest path from v to each node
6. use an array L[0..n-1] for each node w store in L[w] the length of the shortest path from v to w

### Loop invariant
7. for s, L[s] is length of shortest v-> s path
8. edges leaving S go to F
9. for f, L[f] is length of shortest v-> f path using red nodes except for f
0. for b, L[b] = infinity
1. L[v] = 0, L[w] > 0 for w ≠ v

### Improvements
+ Use a heap
+ The set s does not need to be used
+ add backpointer to previous node to also get the path.

### Time
+ for a complete graph O(n^2 log n)
+ for a sparse graph O(n log n)
+ expected time

## Undirected tree
+ only one path to each node from any dnode
+ contains no cycle
+ minimal number of edges to connect all vertices

## Spanning Trees
+ An undirected tree that is a subset of a graph such that it is an undirected tree

### Subtractive method
+ start with the whole graph
+ find a cycle delete one of the edges
+ repeat until there are no more cycles
+ nondeterministic -- does not lead to the same spanning tree every time

### Additive method
+ start with no edges
+ add an edge to an edge that is not yet coonnected
+ uses minimal number of edges method

### Minimum spanning tree
+ the sum of the weights of the edges is the smallest possible

## Greedy Algorithm
+ always picks the optimal choice at each step with hope of finding the best possible answer
+ sometimes can't even proceed

### Kruskal algorithm
+ find the edge with the minimum weight
+ if it forms an edge throw it out
+ otherwise keep it

### Prim's Algorithm
+ starting with any vertex add the min weight edge
+ it must be connected
+ the added edge must combine to form a tree
+ Adjacency queue
    + O(n + m log m) with a standard PQ
    + O(m + n log n) with a fancier PQ
+ O(n^2) with an adjacency matrix

### Conclusions
+ if all edges are distinct these always find the same tree

### Applications
+ can used to draw mazes

## Travelling salesman problem


