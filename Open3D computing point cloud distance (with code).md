###  directory 

 CloudCompare software related operations 

##  Introduction to the algorithm 

##  1. Main function 

   The compute_point_cloud_distance function in Open3D provides a way to calculate the distance from the source point cloud to the target point cloud, computing the distance of the point cloud. That is, it calculates the distance from each point in the source point cloud to the nearest point in the target point cloud. 

##  2. Algorithm source code 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574462185
  ```  
   In the following example, a function is used to calculate the difference between two clouds. Note that this method can also be used to calculate the Chamfer distance between two clouds. 

##  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574462185
  ```  
##  III. Display of results 

 ![avatar](20201229184810352.png) 

##  IV. Remarks 

 ![avatar](20210113084002129.png) 

 The unit of the calculated result here is meters, and the Euclidean distance between the two points is calculated. The distance between the two points measured in the CloudCompare software and the distance between the two points calculated by the code are the same. 

