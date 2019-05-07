## Orthogonal Art Gallery Problem 


### Setting the Stage 

In 1973, Victor Klee came up with the problem of **determining the minimum number of guards sufficient to cover the interior of an *n*-wall art gallery room**. 2 years later, Vasek Chavatal established what was later known as the "Chavatal's Art Gallery Theorem," that **n/3 guards are occasionally necessary and always sufficient to cover a polygon of *n* vertices** [(Chvatal 1975)](https://www.sciencedirect.com/science/article/pii/0095895675900611?via%3Dihub). 

Steve Fisk later derived another sufficiency proof. We will include it here since it is remarkably consise and elegant [(Fisk 1977)](https://www.sciencedirect.com/science/article/pii/009589567890059X). First, the polygon is triangulated. It is known that any outerplanar graph (certainly including triangulation of a polygon) can be 3-colored. The vertices with any one color form a valid guard set, where each triangle of the polygon is guarded by its vertex with that color. Since the three colors partition the n vertices of the polygon, the color with the fewest vertices defines a valid guard set with at most n/3 guards. 

![](/img/img17.JPG)

<p style="text-align: center;"> Courtesy of Professor Greg Aloupis </p>

**In this project, we look at one variation of the problem, where the art gallery is an orthogonal polygon.** An orthogonal polygon is one whose edges are aligned with either horizontal or vertical axes. The edges alternate between horizontal and vertical, and always meet orthogonally, with internal angles of either 90 degrees or 270 degrees. Orthogonal art gallery problem is especially interesting and practical because in real life a lot of galleries are of the shape of orthogonal polygons. For example, below is a floor plan of MoMA, which is an orthogonal polygon. 

![](/img/img16.JPG)

<p style="text-align: center;"> Courtesy of MoMA </p>

The orthogonal art gallery theorem was first formulated and proved by **Kahn, Klawe, and Kleitman** in 1983 [(Kanh *et al.* 1983)](https://epubs.siam.org/doi/abs/10.1137/0604020). It states that **n/4 guards are occasionally necessary and always sufficient to see the interior of an orthogonal art gallery room.**

![](/img/img18.JPG)

### [Groyi's Proof](/gyori.md)
In 1986, Ervin Gyori derived a more compact proof [(Gyori 1986)](https://epubs.siam.org/doi/10.1137/0607051). However, it still remains complex and difficult to grasp. Therefore, this project aims at making it easier to understand by supplying more illustrations and using simpler languages. 
