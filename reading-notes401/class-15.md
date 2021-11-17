# Trees

In this tutorial, we’ll be covering Binary Trees, Binary Search Trees, and K-ary Trees. We will review some common terminology that is shared amongst all of the trees and then dive into specifics of the different types.

## Common Terminology

tree: a data structure that is either a leaf or has two branches.
leaf: a node that has no children.
branch = k: a node that has two children.
its a binary tree if it has only two branches.
Traversals
Depth First Search: DFS is a recursive algorithm that traverses a tree in a pre-order, in-order, or post-order fashion.
Breadth First Search: BFS is an iterative algorithm that traverses a tree in a level-order fashion.

Binary Tree Vs K-ary Trees

- The K-ary tree is a rooted tree, where each node can hold at most k number of children. If the value of k is 2, then this is known as binary tree. The binary tree, or ternary trees are some specialized k-ary trees.

- What is a complete K-ary tree?
  K-ary trees are trees whose internal nodes all have exactly K children. Thus, a full binary tree is a 2-ary tree. The PR Quadtree discussed in Module Spatial is an example of a 4-ary tree. Because K-ary tree nodes have a fixed number of children, unlike general trees, they are relatively easy to implement.
  The K-ary tree is a rooted tree, where each node can hold at most k number of children. ... If the value of k is 2, then this is known as binary tree.
- Big O
  The Big O time complexity for inserting a new node is O(n). Searching for a specific node will also be O(n). Because of the lack of organizational structure in a Binary Tree, the worst case for most operations will involve traversing the entire tree. If we assume that a tree has n nodes, then in the worst case we will have to look at n items, hence the O(n) complexity.
  The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n.
  The Big O space complexity of a BST search would be O(1). During a search, we are not allocating any additional space.
