# Trees

![check](https://i.ibb.co/3Sr9nDw/c.png)
## Terminology

* Node - A Tree node is a component which may contain it’s own values, and references to other nodes
* Root - The root is the node at the beginning of the tree
* K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
* Left - A reference to one child node, in a binary tree
* Right - A reference to the other child node, in a binary tree
* Edge - The edge in a tree is the link between a parent and child node
* Leaf - A leaf is a node that does not have any children
* Height - The height of a tree is the number of edges from the root to the furthest leaf

## Traversals
1. **Depth First** : is where we prioritize going through the depth (height) of the tree first

* **methods for depth first traversal:**
Pre-order: ``root >> left >> right``
In-order: ``left >> root >> right``
Post-order: ``left >> right >> root``
* most common way to traverse through a tree is to use **recursion**

2. **Breadth First**:  iterates through the tree by going through each level of the tree node-by-node. 
* Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. 
* Dequeue the front node, enqueue that node’s left and right nodes, and move to the next new front of the queue.


## Binary Tree Vs K-ary Trees

* **Binary Tree**: Binary Trees restrict the number of children to two (hence our left and right children).
* **K-ary Trees**: Nodes are able have more than 2 child nodes
* **Breadth First Traversal**
Traversing a K-ary tree requires a similar approach to the breadth first traversal. We are still pushing nodes into a queue, but we are now moving down a list of children of length k, instead of checking for the presence of a left and a right child.
* **adding Node**
One strategy for adding a new node to a binary tree is to fill all “child” spots from the top down. To do so, we would leverage the use of breadth first traversal. During the traversal, we find the first node that does not have all it’s children filled, and insert the new node as a child. We fill the child slots from left to righ

## Big O
### The Big O time complexity for inserting a new node is**O(n)**. Searching for a specific node will also be **O(n)**.
 * Because of the lack of organizational structure in a Binary Tree, the worst case for most operations will involve traversing the entire tree. If we assume that a tree has n nodes, then in the worst case we will have to look at n items, hence the O(n) complexity.

### The Big O space complexity for a node insertion using breadth first insertion will be O(w), where w is the largest width of the tree. For example, in the above tree, w is 4.

### A “perfect” binary tree is one where every non-leaf node has exactly two children. The maximum width for a perfect binary tree, is 2^(h-1), where h is the height of the tree. Height can be calculated as log n, where n is the number of nodes.

## A Binary Search Tree (BST)
* BST: is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

* The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). 
*  Big O space complexity of a BST search would be O(1)