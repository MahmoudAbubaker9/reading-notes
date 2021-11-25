# Graphs

A graph is a non-linear data structure that can be looked at as a collection of vertices (or nodes) potentially connected by line segments named edges.

**Terminology:**
1. Vertex: also called a “node”, is a data object that can have zero or more adjacent vertices.
2. Edge: is a connection between two nodes.
3. Neighbor: The neighbors of a node are its adjacent nodes
4. Degree: The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected

* Undirected Graphs : graph where each edge is undirected or bi-directional.

![undirected](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

* Directed Graphs : also called a Digraph is a graph where every edge is directed.

![directed](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)

## Complete vs Connected vs Disconnected

![Complete vs Connected vs Disconnected](https://res.cloudinary.com/practicaldev/image/fetch/s--Y9uFX5E3--/c_limit%2Cf_auto%2Cfl_progressive%2Cq_auto%2Cw_880/https://dev-to-uploads.s3.amazonaws.com/i/pm6c3clylaop6oxfu478.png)

1. **Complete Graphs:** A complete graph is when all nodes are connected to all other nodes.

2. **Disconnected Graphs:** It is a graph in which some node may not have edges.

3. **Connected Graphs :** A connected graph is graph that has all of vertices/nodes have at least one edge.

* It is complelty possible to have standalone nodes or edges (also known as islands) in a graph data structure.

## Acyclic vs Cyclic:

1. **Acyclic Graph:**
An acyclic graph is a directed graph without cycles.

A cycle is when a node can be traversed through and potentially end up back at itself.

![Acyclic Graph](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/threeAcyclic.png)

2. **Cyclic Graphs:**

A Cyclic graph is a graph that has cycles.

![Cyclic Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/cyclic.PNG)

## Traversals

We can use either use Breadth First or Depth First in travelling in the graph.

**Breadth First**

Breadth first traversal is when you visit all the nodes that are closest to the root as possible

**Algorithm:**

1. `Enqueue` the declared start node into the Queue.
2. Create a loop that will run while the node still has nodes present.
3. `Dequeue` the first node from the queue
4. if the Dequeue‘d node has unvisited child nodes, add the unvisited children to `visited` set and insert them into the queue.


**Depth First**

In a depth first traversal, we approach it a bit different than the way we do when working with a depth first traversal of a tree. Similar to how the breadth-first uses a queue, we are going to use a Stack for our depth-first traversal.

**Algorithm:**

1. `Push` the root node into the stack
2. Start a while loop while the stack is not empty
3. `Peek` at the top node in the stack
4. If the top node has unvisited children, mark the top node as visited, and then `Push` any unvisited children back into the stack.
5. If the top node does not have any unvisited children, `Pop` that node off the stack
6. repeat until the stack is empty.

### Real World Uses of Graphs

- Graphs are extremely popular when it comes to it’s uses. Here are just a few examples of graphs in use:

1. GPS and Mapping
2. Driving Directions
3. Social Networks
4. Airline Traffic
5. Netflix uses graphs for suggestions of products













