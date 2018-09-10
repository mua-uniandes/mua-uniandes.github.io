# Binary Indexed Tree

A ***binary indexed tree*** also known as a Fenwick tree can be seen as a dynamic variant of a
prefix sum array. It provides two O(log n) time operations:
* processing a range sum query 
* updating a value.

Even if the name of the structure is a binary indexed tree, the structure is usually represented as an array. When discussing binary indexed trees, we assume that all arrays are one-indexed, because it makes the implementation of the structure easier.

A simple solution is to run a loop from 0 to i-1 and calculate sum of elements. One way of updating a value is doing the following operation: **arr[i] = x**. The first solution takes **O(n) time** and second operation takes **O(1) time**. Another simple solution is to create another array and store sum from start to i at the i’th index in this array. Sum of a given range can now be calculated in O(1) time, but update operation takes O(n) time now. This works well if the number of query operations are large and very few updates.

We construct the Binary Indexed Tree by first initializing all values in array BITree[] as 0. Then we call update() operation for all indexes to store actual sums.


<p align="center">
  <img width="460" height="400" src="https://www.geeksforgeeks.org/wp-content/uploads/BITSum.png">
</p>
