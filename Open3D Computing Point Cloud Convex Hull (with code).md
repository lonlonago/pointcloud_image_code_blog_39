#  First, the basis for realization 

>  The convex hull of a point cloud is the smallest convex set that contains all points. open3d implements the method of computing convex hulls: compute_convex_hull. The implementation of this interface is based on Qhull. The following code first downsamples a point cloud from the point cloud, then calculates the convex hull, and finally visualizes the convex hull with a red line. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574446374
  ```  
#  III. Display of results 

##   1. Primitive point cloud 

 ![avatar]( fbd2aedd0db24c5e871a099df20c81e5.png) 

##   2. Visualization of convex hull 

 ![avatar]( 20200826085139142.png) 

##   3. Convex hull vertex 

 ![avatar]( d8fb2a3584eb4c2390f83d1f2a63f699.png) 

