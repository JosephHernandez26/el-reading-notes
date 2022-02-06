# El Reading Notes of the 401 Variety

## Trees - Reading Notes

### Common Terminology

**Node**

- A Tree node is a component which may contain it’s own values, and references to other nodes

**Root**

- The root is the node at the beginning of the tree

**K**

- A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

**Left**

- A reference to one child node, in a binary tree

**Right**

- A reference to the other child node, in a Binary Tree.

**Edge**

- The edge in a tree is the link between a parent and child node

**Leaf**

- A leaf is a node that does not have any children

**Height**

- The height of a tree is the number of edges from the root to the furthest leaf

#### Traversals

- An important aspect of trees is how to traverse them.

- Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! 

- There are two categories of traversals when it comes to trees:

**1. Depth First**

**2. Breadth First**

#### Depth First

- Depth first traversal is where we prioritize going through the depth (height) of the tree first. There are multiple ways to carry out depth first traversal, and each method changes the order in which we search/print the root.

- Here are three methods for depth first traversal:

**Pre-order**: 

- Pre-order means that the root has to be looked at first. In our case, looking at the root just means that we output its value. When we call preOrder for the first time, the root will be added to the call stack:

root >> left >> right

- This means that we will output the root.value out to the console. Then, our next block of code instructs us to check if our root has a left node set. If the root does, we will then send the left node to our preOrder method recursively.

**In-order**:

left >> root >> right

**Post-order**:

left >> right >> root

The most common way to traverse through a tree is to use recursion. With these traversals, we rely on the call stack to navigate back up the tree when we have reached the end of a sub-path.

#### Breadth First

- Breadth first traversal iterates through the tree by going through each level of the tree node-by-node.

- Traditionally, breadth first traversal uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree. Let’s break down the process.

#### Binary Tree Vs K-ary Trees

- In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

- There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows.

- Binary Tree Vs K-ary Trees
In all of our examples, we’ve been using a Binary Tree. Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

There is no specific sorting order for a binary tree. Nodes can be added into a binary tree wherever space allows.

#### Binary Search Trees

- A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

**Searching a BST**

- Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.

[The Source of all this knowledge](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

 <a href="#top">Take Me To The Repo!!</a>
