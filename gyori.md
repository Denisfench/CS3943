## Gyori's Proof

### Claim
*[n/4]* guards are sometimes necessary, but always sufficient to guard the interior of an *n*-wall **orthogonal** art gallery. 

### A Stronger Claim 
This proof will instead prove a stronger claim than the one above, that:    

**if P is an orthogonal polygon of *n* vertices, then P can be partitioned into at most [n/4] orthogonal polygons of 4 or 6 vertices.** 

To see why this implies the previous claim, we can see that orthognal polygons of 4 or 6 vertices are of unique shapes, being rectangular or in the shape of a capital letter "L" respectively. Becasue the both shapes are convex polygons, one guard is sufficient to guard each. 

![](/img/img1.jpg)

### Simple Facts about Orthogonal Polygons 
By definition, orthogonal polygons are polygons whose sides are parallel to either the horizontal or the vertical axes. 
1. Therefore, the internal angles of an orthogonal polygons are of 90 degrees (**convex**) or 270 degrees (**concave**). 
2. The sides of an orthogonal polygon are alternatively horizontal and vertical, which means *n* must be even. 

### An Inductive Proof 
If *n* is 4 or 6, we have nothing to prove (base case). Since *n* must be even, let's assumet that *n* >= 8. 

#### Case 1 (Very Easy) 
There are two vertices of P that can be connected by a horizontal or vertical segment without crossing the boundaries of P. If this is the case, we can cut P along that very segment and we will obtain 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> + n<sub>2</sub> = n**. We are done by inductive hypothesis. 

![](/img/img2.jpg)

#### Case 2 (Easy) 
This is the case where *n* = 4k, where k is some integer greater than 1. If we take a concave vertex V of the polygon P and cut P horizontally through the boundary of P, we will obtain 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> + n<sub>2</sub> = n+2**. It is becasue the cut creates a new vertex, W, which is used by both P<sub>1</sub> and P<sub>2</sub>. We are done by inductive hypothesis because: 

**n<sub>1</sub>/4 + n<sub>2</sub>/4 <= (n+2)/4 = n/4** 

![](/img/img3.jpg)


