---
id: geometry
title: Geometry
toc_max_heading_level: 2
---

## Introduction

Geometry is a branch of mathematics that is concerned with properties of space that are related with distance, shape, size, and relative position of figures. Advanced geometry (e.g. 3D geometry) is not taught in most Computer Science courses, so you can expect that you will only be asked on 2D geometry.

In algorithm interviews, geometry is usually not be the focus of the problem (you're not being evaluated on mathematics after all). You typically have to use other algorithms and/or data structures in the problem.

## Corner cases

- Zero values. This always gets people.

## Techniques

### Distance between two points

When comparing the between two points, using dx<sup>2</sup> + dy<sup>2</sup> is sufficient. It is unnecessary to square root the value. Examples: [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin/)

### Overlapping circles

To find out if two circles overlap, check that the distance between the two centers of the circles is less than the sum of their radii.

### Overlapping rectangles

Two rectangles overlap if the following is true:

```py
overlap = rect_a.left < rect_b.right and \
  rect_a.right > rect_b.left and \
  rect_a.top > rect_b.bottom and \
  rect_a.bottom < rect_b.top
```

Here's a [nice visualization](https://silentmatt.com/rectangle-intersection/). Examples: [Rectangle Overlap](https://leetcode.com/problems/rectangle-overlap/)

## Sample questions

- You have a plane with lots of rectangles on it, find out how many of them intersect.
- Which data structure would you use to query the k-nearest points of a set on a 2D plane?
- Given many points, find k points that are closest to the origin.
- How would you triangulate a polygon?

## Recommended questions

- [Rectangle Overlap](https://leetcode.com/problems/rectangle-overlap/)
- [K Closest Points to Origin](https://leetcode.com/problems/k-closest-points-to-origin/)
- [Rectangle Area](https://leetcode.com/problems/rectangle-area/)

## Recommended courses

import AlgorithmCourses from '../\_courses/AlgorithmCourses.md'

<AlgorithmCourses />
