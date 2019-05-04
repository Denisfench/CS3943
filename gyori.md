## Gyori's Proof

### Claim
*[n/4]* guards are sometimes necessary, but always sufficient to guard the interior of an *n*-wall **orthogonal** art gallery. 

### A Stronger Claim 
This proof will instead prove a stronger claim than the one above, that:    

**if P is an orthogonal polygon of *n* vertices, then P can be partitioned into at most [n/4] orthogonal polygons of 4 or 6 vertices.** 

To see why this implies the previous claim, we can see that orthognal polygons of 4 or 6 vertices are of unique shapes, being rectangular or in the shape of a capital letter "L" respectively. Becasue both shapes are convex polygons, one guard is sufficient to guard each. 

![](/img/img1.jpg)

### Some Facts about P(Orthogonal Polygon)
1. The internal angles of P are of 90 degrees (**convex**) or 270 degrees (**concave**). 
2. The sides of P are alternatively horizontal and vertical, which means *n* must be even. 
3. For P, [the number of concave vertices is 4 less than the number of convex vertices.](/convexity.md)

### Base Case of An Inductive Proof 
If *n* is 4 or 6, we have nothing to prove (base case). Since *n* must be even, let's assumet that *n* >= 8. 

### Case 1 (Easy) 
There are two vertices of P that can be connected by a horizontal or vertical segment without crossing the boundaries of P. If this is the case, we can cut P along that very segment and we will obtain 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> + n<sub>2</sub> = n**. We are done by inductive hypothesis. 

![](/img/img2.jpg)

### Case 2 (Easy) 
This is the case where *n* = 4k, where k is some integer > 1. If we take a concave vertex V of the polygon P and cut P horizontally through the boundary of P, we will obtain 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> + n<sub>2</sub> = n+2**. It is becasue the cut creates a new vertex, W, which is used by both P<sub>1</sub> and P<sub>2</sub>. We are done by inductive hypothesis because: 

**n<sub>1</sub>/4 + n<sub>2</sub>/4 <= (n+2)/4 = n/4** 

![](/img/img3.jpg)

### Case 3 (Hard) 
We are left with the case where *n* = 4k+2, where k is some integer > 1. According to fact 3, P must have **2k+3** convex vertices and **2k-1** concave vertices. Therefore, there exist two neighboring convex vertice in P which we can call X and Y. If we move the side XY orthogonally through the interior of P as far as P's boundary, let X<sub>1</sub> and Y<sub>1</sub> denote the images of X and Y, respectively, under the translation. 

Suppose that upon our cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub> out of P, we should obtain either 1 or 2 polygons. The only scenario where upon our cutting we will obtain more than 2 polygons is shown below. However, in this scenario, a horizontal segement can be connected between A and B without crossing the bounday of P, which means it is in **Case 1**. Because we are in **Case 3**, we cannot find such A and B. As proved by contradiction, we will obtain either 1 or 2 polygons upon cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub>. 

![](/img/img4.jpg) 


#### Scenario A: 2 Polygons
In the case where we obtain 2 polygons upon cutting the rectangle XYX<sub>1</sub>Y<sub>1</sub>, X<sub>1</sub>Y<sub>1</sub> only intersects with one side UV of P. There are three different relations between the side UV and the segment X<sub>1</sub>Y<sub>1</sub>. 

![](/img/img5.jpg)

In each relation above, we may cut P along the purple segment *a* or *b*. One of the cut will yield 2 new polygons P<sub>1</sub> and P<sub>2</sub> of n<sub>1</sub> and n<sub>2</sub> vertices, respectively, such that **n<sub>1</sub> = 4k<sub>1</sub> + 2, n<sub>2</sub> = 4k<sub>2</sub> + 2, and k = k<sub>1</sub> + k<sub>2</sub>**. Therefore we are done by the inductive hypothesis. 

Here are 3 examples, one for each relation: 

Example 1 covers the relation where X<sub>1</sub>Y<sub>1</sub> contains UV, where *n* = 18 and k = 4. As established earlier, P must have **2k-1** concave vertices. Suppose that concave vertices i and j are now blocked by the segment a and b, the green polygon and grey polygon should have in total **2k-3** concave vertices. Becasue **2k-3** is odd, it implies that either the green polygon or the purple polygon has an even number of concave vertices. If we cut along segment a, j will be freed to join the grey polygon. Similary, if we cut along segment b, i will be freed to join the green polygon. Therefore, if the green polygon has an even number of concave vertices, we should cut along segment b; if the grey polygon has an even number of concave vertices, we should cut along segment a. 

![](/img/img6.jpg)

Here the grey polygon has an even number of concave vertices, which suggests that we should cut along segment a. After performing such cut, we will find that n<sub>1</sub>1 = 10, k<sub>1</sub>=2, n<sub>2</sub>=10, k<sub>2</sub>=2, which means **n<sub>1</sub> = 4k<sub>1</sub> + 2, n<sub>2</sub> = 4k<sub>2</sub> + 2**. We also find that after the cut, 2 new vertices are produced: 
  **4k<sub>1</sub> + 2 + 4k<sub>2</sub> + 2 = 4k + 2 + 2** 
  **k<sub>1</sub> + k<sub>2</sub> = k** 

![](/img/img7.jpg)

If we cut along B, **k<sub>1</sub> + k<sub>2</sub> > k**. Therefore, the inductive hypothesis won't work. 

![](/img/img8.jpg)

#### Scenario B: 1 Polygons


### [Return to Index Page](/CS3943)



