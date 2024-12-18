# Abstract Data Types
Abstract Data Types (ADTs) are high-level abstractions that define data structures based on their behavior, rather than their specific implementation. They specify what operations a data structure should support but leave the how of implementation open to the programmer.

Programmers can choose the most efficient implementation for a specific scenario without affecting the overall functionality. By hiding implementation details, ADTs create a more generic and user-friendly interface, leading to cleaner and more understandable code.

## Vectors
A vector is a single-dimensional data structure used for storing data. Think of it as a container that holds a sequence of elements in a linear order. Vectors can be created using lists or numpy arrays.

- Accessing and adding values to a vector has a time complexity of _O(1)._
- Finding an element in a vector has a time complexity of _O(n)_ because, in the worst case, you might have to scan through all elements.

## Stacks
A stack is a linear data structure that follows the Last-In, First-Out (LIFO) principle, meaning the last element added to the stack is the first one to be removed. You can also think of it as First-In, Last-Out (FILO). Imagine a stack of plates; you can only add or remove a plate from the top.

- The Push method adds an element to the top of the stack. Think of this as placing a new plate on top of the stack. It has a time complexity of _O(1)._
- The pop removes and returns the element at the top of the stack. Think of this as taking the top plate off the stack. It has a time complexity of _O(1)._

## Queues
A queue is a linear data structure that follows the First-In, First-Out (FIFO) principle. This means that the first element added to the queue is the first one to be removed. Think of it like a line at a store; the first person in line is the first one to be served.

- The enqueue methods add an element to the rear (end) of the queue. This is like a new person joining the end of the line. It has a time complexity of _O(1)._
- The dequeue removes and returns the element at the front (beginning) of the queue. This is like the person at the front of the line being served and leaving. It has a time complexity of _O(1)._

## Trees
A tree is a non-linear data structure that organizes data in a hierarchical manner. It consists of a finite set of nodes connected by branches. While designing algorithms, we use trees wherever we need to represent hierarchical relationships among the data elements that we need to store or process.

| **Root node**             | A node with no parent is called the root node. For example, in the following diagram, the root node is A. In algorithms, usually, the root node holds the most important value in the tree structure.                                                                                                          |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Level of a node**       | The distance from the root node is the level of a node. For example, in the following diagram, the level of nodes D, E, and F is two.                                                                                                                                                                          |
| **Siblings nodes**        | Two nodes in a tree are called siblings if they are at the same level. For example, if we check the following diagram, nodes B and C are siblings.                                                                                                                                                             |
| **Child and parent node** | Node F is a child of node C if both are directly connected and the level of node C is less than node F. Conversely, node C is a parent of node F. Nodes C and F in the following diagram show this parent-child relationship.                                                                                  |
| **Degree of a node**      | The degree of a node is the number of children it has. For example, in the following diagram, node B has a degree of two.                                                                                                                                                                                      |
| **Degree of a tree**      | The degree of a tree is equal to the maximum degree that can be found among the constituent nodes of a tree. For example, the tree presented in the following diagram has a degree of two.                                                                                                                     |
| **Subtree**               | A subtree of a tree is a portion of the tree with the chosen node as the root node of the subtree and all of the children as the nodes of the tree. For example, a subtree at node E of the tree presented in the following diagram consists of node E as the root node and nodes G and H as the two children. |
| **Leaf node**             | A node in a tree with no children is called a leaf node. For example, in the following figure, nodes D, G, H, and F are the four leaf nodes.                                                                                                                                                                   |
| **Internal node**         | Any node that is neither a root nor a leaf node is an internal node. An internal node will have at least one parent and at least one child node.                                                                                                                                                               |

### Types of Trees

- Binary Tree: A tree where each node has a maximum of two children, often referred to as the left and right children.
- Full Tree: A tree in which every node (except leaf nodes) has the same degree, equal to the degree of the tree.
- Perfect Tree: A special case of a full tree where all leaf nodes are at the same level.
- Ordered Tree: A tree where the children of each node are arranged in a specific order, often determined by some criteria, such as ascending or descending value.