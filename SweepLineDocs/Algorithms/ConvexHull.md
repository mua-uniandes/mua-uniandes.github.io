# Convex Hull Problems

A ***convex hull*** is the smallest convex polygon that contains all points of a given
point set. Here convexity means that a line segment between any two vertices of the
polygon is completely inside the polygon.

**NOTE:** There are many efficient algorithms for constructing convex hulls. Perhaps the
simplest among them is Andrew’s algorithm

**Andrew's Algorithm:**
The algorithm first determines the leftmost and rightmost points in the set, and then
constructs the convex hull in two parts: first the upper hull and then the lower hull.
Both parts are similar, so we can focus on constructing the upper hull.
First, we sort the points primarily according to x coordinates and secondarily
according to y coordinates. After this, we go through the points and add each point
to the hull. Always after adding a point to the hull, we make sure that the last line
segment in the hull does not turn left. As long as it turns left, we repeatedly remove
the second last point from the hull.


**Divide and Conquer Algorithm:**
Given the set of points for which we have to find the convex hull. Suppose we know the convex hull of the left half points and the right half points, then the problem now is to merge these two convex hulls and determine the convex hull for the complete set. This can be done by finding the upper and lower tangent to the right and left convex hulls.
Recursion comes into the picture, we divide the set of points until the number of points in the set is very small, say 5, and we can find the convex hull for these points by the brute algorithm. The merging of these halves would result in the convex hull for the complete set of points.

<p align="center">
  <img width="360" height="120" src="https://cdncontribute.geeksforgeeks.org/wp-content/uploads/Convex_hull_1.jpg">
</p>

