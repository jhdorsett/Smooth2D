This is a partial port of  [Darren Engwirda's MATLAB Mesh2D package (2017).](https://github.com/dengwirda/mesh2d/tree/main) Python refactorization by J. Dorsett (2024).

Darren Engwirda describes the functionality in his Smooth2.m: 

"This routine is loosely based on the DISTMESH algorithm, employing a "spring-based" analogy to redistribute mesh vertices. Such an approach is described in: P.O. Persson and Gilbert Strang. "A simple mesh generator in MATLAB." SIAM review 46(2) 2004, pp: 329--345. Details of the algorithm used here are somewhat different, with an alterative spring-based update employed, in addition to hill-climbing element quality guarantees, and vertex density controls."

Smooth2D is a powerful 2D mesh smoothing algorithm that we use to generate meshes from a user-generated set of nodes and vertices created using Delaunay triangulation. Smooth2D accepts a nodeset (`vert`), triangulation set (`tria`), and a connectivity set (`conn`), which references edges that are to remain fixed. 
