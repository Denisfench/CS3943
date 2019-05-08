## Gyori's Proof

### Claim
*[n/4]* guards are sometimes necessary, but always sufficient to guard the interior of an *n*-wall **orthogonal** art gallery. 

### A Stronger Claim 
This proof will instead prove a stronger claim than the one above, that:    

**if P is an orthogonal polygon of *n* vertices, then P can be partitioned into at most [n/4] orthogonal polygons of 4 or 6 vertices.** 

To see why this implies the previous claim, we can see that orthogonal polygons of 4 or 6 vertices are of unique shapes, being rectangular or in the shape of a capital letter "L" respectively. Because both shapes are convex polygons, one guard is sufficient to guard each. 

![](/img/img1.jpg)

### Some Facts about P(Orthogonal Polygon)
1. The internal angles of P are of 90 degrees (**convex**) or 270 degrees (**concave**). 
2. The sides of P are alternately horizontal and vertical, which means *n* must be even. 
3. For P, [the number of concave vertices is 4 less than the number of convex vertices.](/convexity.md)

### Base Case of An Inductive Proof 
If *n* is 4 or 6, we have nothing to prove (base case). Since *n* must be even, let's assume that *n* >= 8. 

### Case 1 (Easy) 
There are two vertices of P that can be connected by a horizontal or vertical segment without crossing the boundaries of P. If this is the case, we can cut P along that very segment and we will obtain 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> + n<sub>2</sub> = n**. We are done by inductive hypothesis. 

![](/img/img2.jpg)

### Case 2 (Easy) 
This is the case where *n* = 4k, where k is some integer > 1. If we take a concave vertex V of the polygon P and cut P horizontally through the boundary of P, we will obtain 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> + n<sub>2</sub> = n+2**. It is becasue the cut creates a new vertex, W, which is used by both P<sub>1</sub> and P<sub>2</sub>. We are done by inductive hypothesis because: 

**n<sub>1</sub>/4 + n<sub>2</sub>/4 <= (n+2)/4 = n/4** 

![](/img/img3.jpg)

### Case 3 (Hard) 
We are left with the case where *n* = 4k+2, where k is some integer > 1. According to the fact 3, P must have **2k+3** convex vertices and **2k-1** concave vertices. Therefore, there exist two neighboring convex vertice in P which we can call X and Y. If we move the side XY orthogonally through the interior of P as far as P's boundary, let X<sub>1</sub> and Y<sub>1</sub> denote the images of X and Y, respectively, under the translation. 

Suppose that upon our cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub> out of P, we should obtain either 1 or 2 polygons. The only scenario whereupon our cutting we will obtain more than 2 polygons is shown below. However, in this scenario, a horizontal segment can be connected between A and B without crossing the boundary of P, which means it is in **Case 1**. Because we are in **Case 3**, we cannot find such A and B. As proved by contradiction, we will obtain either 1 or 2 polygons upon cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub>. 

![](/img/img4.jpg) 


#### Scenario I: 2 Polygons
In the case where we obtain 2 polygons upon cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub>, X<sub>1</sub>Y<sub>1</sub> only intersects with one side UV of P. There are 3 different relations between the side UV and the segment X<sub>1</sub>Y<sub>1</sub>. 

![](/img/img5.jpg)

In each relation above, we may cut P along the purple segment *a* or *b*. One of the cut will yield 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> = 4k<sub>1</sub> + 2, n<sub>2</sub> = 4k<sub>2</sub> + 2, and k = k<sub>1</sub> + k<sub>2</sub>**. Therefore we are done by the inductive hypothesis. 

Here are 3 examples, one for each relation: 

### [Example 1: X<sub>1</sub>Y<sub>1</sub> contains UV](/2PolygonsEx1.md)

### [Example 2: UV contains X<sub>1</sub>Y<sub>1</sub>](/2PolygonsEx2.md)

### [Example 3: UV overlaps with X<sub>1</sub>Y<sub>1</sub>](/2PolygonsEx3.md)

#### Scenario II: 1 Polygons

In the case where we obtain only 1 polygon upon cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub>, XX<sub>1</sub> or YY<sub>1</sub> must be a side of P. Here we assume that XX<sub>1</sub> is a side of P and X<sub>1</sub> = U. 

There are 2 relations:

When X<sub>1</sub>Y<sub>1</sub> contains the side X<sub>1</sub>V and YY<sub>1</sub> contains the side YZ of P, we cut P along the segments a and b obtaining P<sub>1</sub> (the L-shaped one) of 6 vertices and P<sub>2</sub> (the rest) of 4k-2 vertices. It is easy to see why P<sub>2</sub> must have 4k-2 vertices: the cutting reduces 5 green vertices from it and adds 1 vertex to it. Therefore, 4k+2-5+1 = 4k-2. 4k-2 = 4(k-1) + 2. We are done by inductive hypothesis. 

![](/img/img15.jpg)

### [A walkthrough when n = 14](/walkthrough.md)

### [Return to Index Page](/CS3943)



