# Implementation: Trees


* binary tree is a tree data structure in which each node has at most two children, which are referred to as the left child and the right child. ... It is also possible to interpret a binary tree as an undirected, rather than a directed graph, in which case a binary tree is an ordered, rooted tree

![binary tree](https://media.geeksforgeeks.org/wp-content/cdn-uploads/binary-tree-to-DLL.png)

-----------------------------------


*  K-ary trees are trees whose internal nodes all have exactly K children. Thus, a full binary tree is a 2-ary tree. The PR Quadtree discussed in Module <Spatial> is an example of a 4-ary tree. Because K-ary tree nodes have a fixed number of children, unlike general trees, they are relatively easy to implement.

![ K-ary trees](https://www.researchgate.net/profile/Stan-Zdonik/publication/220538512/figure/fig1/AS:394041536598031@1470958231917/Example-of-a-k-ary-tree-with-k-4.png)

---------------------

* A binary search tree (BST) is a binary tree where each node has a Comparable key (and an associated value) and satisfies the restriction that the key in any node is larger than the keys in all nodes in that node's left subtree and smaller than the keys in all nodes in that node's right subtree

![Binary Search Trees,](https://media.geeksforgeeks.org/wp-content/uploads/BSTSearch.png)



--------------------------------

* Traversals : 
   * Traversing a tree allows us to search for a node, print out the contents of a tree 📔
      * ategories of traversals when it comes to trees:

          * Depth First :Pre-order:
           root >> left >> right

In-order: left >> root >> right

Post-order: left >> right >> root
        
        
        
 * Breadth First
           

  * The K-ary tree is a rooted tree, where each node can hold at most k number of children. ... If the value of k is 2, then this is known as binary tree         

  ![trees](https://media.geeksforgeeks.org/wp-content/uploads/20200219144238/General-Tree-vs-Binary-Tree.png)


  **Big O**

* The Big O time complexity of a Binary Search Tree’s insertion and search operations is O(h), or O(height). In the worst case, we will have to search all the way down to a leaf, which will require searching through as many nodes as the tree is tall. In a balanced (or “perfect”) tree, the height of the tree is log(n). In an unbalanced tree, the worst case height of the tree is n.

* The Big O space complexity of a BST search would be O(1).


 #### &copy; Dima Alabsi; 2021
