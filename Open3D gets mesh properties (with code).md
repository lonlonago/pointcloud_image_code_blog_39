###  directory 

 Let's first take a look at the implementation in CloudCompare software 

##  First, the main function analysis 

   Triangular meshes have several properties that can be tested with open3d. An important property is the manifold property, which can be used is_edge_manifold to test whether the mesh is an edge manifold and is_vertex_manifold to test whether all vertices are manifolds. If a triangular mesh is an edge manifold and each edge includes one or two triangles. The is_edge_manifold function has a bool-type parameter allow_boundary_edges used to specify whether edges of the boundary are allowed (if true, a non-manifold edge is defined as an edge with more than two adjacent triangles, otherwise each side that is not adjacent to two triangles is defined as a non-manifold.). In addition, a triangular mesh is a vertex manifold if the fixed-point star of the vertex is an edge-manifold and an edge-connected one. For example, two or more faces may be connected by only one vertex instead of an edge. Another property is the self-intersection test. If there are triangles in one mesh that intersect with another, is_self_intersecting this function returns true. A watertight mesh can be defined as an edge-manifold), a vertex manifold (vertex manifold) and not self-intersecting (not self-intersecting). This detection is implemented in open3d via the is_watertight interface. We can also test whether a mesh is orientable by is_orientable (triangles can be oriented by all normals pointing out) The following code tests these properties and visualizes them. Non-manifold edges are shown in red, boundary edges are identified in green, non-manifold vertices are shown in green dots, and self-intersecting triangles are shown in pink. 

##  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574476907
  ```  
##  III. Display of results 

 ![avatar](20201204160752706.png) 

