## Example 1: X<sub>1</sub>Y<sub>1</sub> contains UV

Example 1 covers the relation where X<sub>1</sub>Y<sub>1</sub> contains UV, where *n* = 18 and k = 4. As established earlier, P must have **2k-1** concave vertices. Suppose that concave vertices i and j are now blocked by the segment a and b, the green polygon and grey polygon should have in total **2k-3** concave vertices. Because **2k-3** is odd, it implies that either the green polygon or the purple polygon has an even number of concave vertices. If we cut along segment a, j will be freed to join the grey polygon. Similarly, if we cut along segment b, i will be freed to join the green polygon. Therefore, if the green polygon has an even number of concave vertices, we should cut along segment b; if the grey polygon has an even number of concave vertices, we should cut along segment a. 

![](/img/img6.jpg)

Here the grey polygon has an even number of concave vertices, which suggests that we should cut along segment a. After performing such cut, we will find that n<sub>1</sub>1 = 10, k<sub>1</sub>=2, n<sub>2</sub>=10, k<sub>2</sub>=2, which means **n<sub>1</sub> = 4k<sub>1</sub> + 2, n<sub>2</sub> = 4k<sub>2</sub> + 2**. We also find that after the cut, 2 new vertices are produced: 
  **4k<sub>1</sub> + 2 + 4k<sub>2</sub> + 2 = 4k + 2 + 2** 
  **k<sub>1</sub> + k<sub>2</sub> = k** 

![](/img/img7.jpg)

If we cut along B, **k<sub>1</sub> + k<sub>2</sub> > k**. Therefore, the inductive hypothesis won't work. 

![](/img/img8.jpg)

### [Back to Groyi's Proof](/gyori.md)
