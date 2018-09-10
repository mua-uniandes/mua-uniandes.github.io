# Intersection Points
Given a set of n line segments, each of them being either horizontal or vertical,
consider the problem of counting the total number of intersection points.
It is easy to solve the problem in **O(n2)** time, because we can go through all
possible pairs of line segments and check if they intersect. However, we can solve
the problem more efficiently in **O(n log n)** time using a sweep line algorithm and a
range query data structure. The idea is to process the endpoints of the line segments
from left to right and focus on three types of events:
* Horizontal segment Begins
* Horizontal segment ends
* Vertical segment

After creating the events, we go through them from left to right and use a data
structure that maintains the y coordinates of the active horizontal segments.

<p align="center">
  <img width="460" height= 520" src="https://user-images.githubusercontent.com/35730663/45299161-53631600-b4d0-11e8-87ed-55880d7fd408.png">
</p>
