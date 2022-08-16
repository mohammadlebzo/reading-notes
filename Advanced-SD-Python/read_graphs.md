# Read: Graphs

### Definition:

Graphs are non-linear data structure that consist of a set of nodes that are connected by edges.

### Some common information about graphs:

Some common terminologies:

| Term | Meaning |
|------|---------|
| Vertex | these are the nodes, and they can connect to zero or more nodes |
| Edge | connecting line between two nodes |
| Neighbor | a neighbor of a node is the node that is connected to it |
| Degree | a degree of a vertex is the number of edges connected to that vertex |

**Traversal techniques are**:
- *Breadth First*
- *Depth First*

### Kinds of graphs:

- **Undirected Graphs**: These kinds of graphs take a shape without a direction, meaning that they are connected without rule on how to be traversed.

- **Directed Graphs (Digraph)**: These kinds of graphs always move in a specific direction, meaning that they can traversed in a specific way and only in that way.

- **Complete Graphs**: A graph is a complete graph when all it's nodes are connected with each other.

- **Connected Graphs**: A graph is a connected graph when all it's nodes are connected with at least one edge.

- **Disconnected Graphs**: A graph is a disconnected graph when there are some nodes that don't have edges.

- **Acyclic Graph**: this kind of graph does not have any cycles within it, which means unlike undirected and directed graphs, nodes don't end up back at itself.


- **Cyclic Graphs**: this kind of graph starts and ends at the same point, completing a full circle.

### Graph Representation Techniques:

- **Adjacency Matrix**: this representation results in a binary 2d array, connections are represented using **ones**, and no connection is **zero**.

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjMatrix.PNG)

([source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html#:~:text=This%20is%20what%20an%20adjacency%20matrix%20looks%20like%3A))

**Notes**:

1. The size of this representation is **n*n**.
2. Few connections within a representation is called a **spase graph**.
3. Many connections within a representation is called a **dense graph**.

- **Adjacency List**: this representation uses a linked list representation of all the connected nodes.

![](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/AdjList.PNG)

([source](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html#:~:text=This%20is%20what%20an%20Adjacency%20List%20looks%20like))


