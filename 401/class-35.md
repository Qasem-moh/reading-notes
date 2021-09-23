# Graphs

### graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

* **Vertex** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
* **Edge** - An edge is a connection between two nodes.
* **Neighbor** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
* **Degree** - The degree of a vertex is the number of edges connected to that vertex.

## Undirected & Directed
* An **Undirected** Graph is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction. There are no “directions” given to point to specific vertices. The connection is bi-directional

* A **Directed** Graph also called a Digraph is a graph where every edge is directed. has arrows pointing to specific nodes. Each node is directed at another node with a specific requirement of what node should be referenced next.

## Complete vs Connected vs Disconnected
* **Complete** Graphs A complete graph is when all nodes are connected to all other nodes.
* **Connected** A connected graph is graph that has all of vertices/nodes have at least one edge.
* **Disconnected** A disconnected graph is a graph where some vertices may not have edges.It is complelty possible to have standalone nodes or edges (also known as islands) in a graph data structure.


## Acyclic vs Cyclic
* **Acyclic Graph**  An acyclic graph is a directed graph without cycles.
* cycle is when a node can be traversed through and potentially end up back at itself.
Cyclic Graphs
* **Cyclic** graph is a graph that has cycles.

## Graph Representation
   1. Adjacency Matrix
   2. Adjacency List

## Weighted Graphs
A weighted graph is a graph with numbers assigned to its edges. These numbers are called weights.

## Traversals
  1. Breadth First
  2. Depth First

## Uses 
 1. GPS and Mapping
 2. Driving Directions
 3. Social Networks
 4. Airline Traffic
 5. Netflix uses graphs for suggestions of products
