## Orthogonal Art Gallery Probelm 


### Setting the Stage 

In 1973, Victor Klee came up with the problem of determing the minimum number of guards sufficient to cover the interior of an *n*-wall art gallery room. 2 years later, Vasek Chavatal established what was later known as the "Chavatal's Art Gallery Theorem," that n/3 guards are occasioanlly necessary and always sufficient to cover a polygon of *n* vertices [(Chvatal 1975)](https://www.sciencedirect.com/science/article/pii/0095895675900611?via%3Dihub). 

Steve Fisk later derived another sufficiency proof. We will include it here since it is remarkably consice and elegant [(Fisk 1977)](https://www.sciencedirect.com/science/article/pii/009589567890059X). First, the polygon is triangulated. It is known that any outerplanar graph (certainly including triangulation of a polygon) can be 3-colored. The vertices with any one color form a valid guard set, where each triangle of the polygon is guarded by its vertex with that color. Since the three colors partition the n vertices of the polygon, the color with the fewest vertices defines a valid guard set with at most n/3 guards. 

In this project, we look at one variation of the problem, where the art gallery is an orthogonal polygon. An orthogonal polygon is one whose edges are alined with either horozontal or vertical axes. The edges alternate between horizontal and vertical, and always meet orthogonally, with internal angles of either 90 degree or 270 degree. Orthogonal art gallery problem is especially interesting and practical because in real life a lot of galleries are of the shape of orthogonal polygons. 

The orthogonal art gallery thorem was first formualted and proved by Kahn, Klawe, and Kleitman in 1983 [(Kanh *et al.* 1983)](https://epubs.siam.org/doi/abs/10.1137/0604020). It states that n/4 guards are occasionally necessary and always sufficient to see the interior of an orthogonal art gallery room. 3 years later, Ervin Gyori derived a more succinct proof [(Gyori 1986)](https://epubs.siam.org/doi/10.1137/0607051). However, both proofs still remain complex and difficult to grasp. Therefore, this project aims at making the proofs easier to understand by supplying more illustrations and using simpler languages. 
