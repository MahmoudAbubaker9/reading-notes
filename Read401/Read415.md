# Trees

* A tree is a representation of the non-linear data structure. A tree can be shown using different user-defined or primitive types of data.

* We can use arrays, and classes connected lists or other kinds of data structures to implement the tree. It is a group of interrelated nodes.

### Common Terminology

![tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

1. Node - A Tree node is a component which may contain it’s own values, and references to other nodes
2. Root - The root is the node at the beginning of the tree
3. K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
4. Left - A reference to one child node, in a binary tree
5. Right - A reference to the other child node, in a binary tree
6. Edge - The edge in a tree is the link between a parent and child node
7. Leaf - A leaf is a node that does not have any children
8. Height - The height of a tree is the number of edges from the root to the furthest leaf

### Traversals

Traversing a tree allows us to search for a node, print out the contents of a tree, and much more.

**There are two categories of traversals:**

```
Consider the tree:

    A
   / \
  B   C
 /   / \
D   E   F

```


1. Depth First : A depth first traversal would visit the nodes in this order
```
A, B, D, C, E, F
```
Notice that you go all the way down one leg before moving on.

and there is three methods for depth first traversal:

Pre-order: root >> left >> right
In-order: left >> root >> right
Post-order: left >> right >> root

2. Breadth First : Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

```
A, B, C, D, E, F
```

The difference between the two traversal orders lies in the choice of Container.

For depth first use a stack. (The recursive implementation uses the call-stack...)
For breadth-first use a queue.

### Binary Tree Vs K-ary Trees

Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

K-ary Trees If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

### Adding a node

* It does not matter where to add new node in tree.
* It will go down to the children and start adding from left to right.

### Big O
 
 1. The Big O time complexity for inserting a new node is O(n).
 2. The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree.



### Binary Search Trees (BST)

* In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

* The best way to approach a BST search is with a while loop. ‘ We cycle through the while loop until we hit a leaf, or until we reach a match with what we’re searching for.

Reference Site :
[Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)


