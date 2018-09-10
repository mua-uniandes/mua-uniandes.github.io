# Segment Tree

Asegment tree is a data structure that provides **two O(log n) time operations**: processing
a range query and updating an array value. Segment trees support sum queries,
minimum queries, and many other queries.
The root of the Segment Tree represents the whole array **A[0:N-1]** . Then it is broken down into two half intervals or segments and the two children of the root in turn represent the **A[0:(N-1)/2]** and **A[(N-1)/2+1:(N-1)]** . So in each step, the segment is divided into half and the two children represent those two halves. So the height of the segment tree will be ***logN*** . There are **N** leaves representing the **N** elements of the array. The number of internal nodes is ***N-1***. So, a total number of nodes are ***2XN-1***.

**Once the Segment Tree is built, its structure cannot be changed.**

Since a Segment Tree is a binary tree, a simple linear array can be used to represent this structure.  It is safe to assume that the size of the array is a power of two, and zero-based indexing is used, because it is convenient to build a segment tree for such an array. If the size of the array is not a power of two, we can always append extra elements to it.

## Methods
* For ***update(),***  search the leaf that contains the element to update. This can be done by going to either on the left child or the right child depending on the interval which contains the element. Once the leaf is found, it is updated and again use the bottom-up approach to update the corresponding change in the path from that leaf to the root. In other words, After an array update, we should update all nodes whose value depends on the updated value.
* To make a ***query(),***  on the Segment Tree, select a range from *L*  to *R* (which is usually given in the question). Recurse on the tree starting from the root and check if the interval represented by the node is completely in the range from *L*  to *R*  . If the interval represented by a node is completely in the range from *L*  to *R* , return that node’s value.

<p align="center">
  <img width="360" height="260" src="https://www.geeksforgeeks.org/wp-content/uploads/segment-tree1.png">
</p>
