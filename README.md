#  First, the principle of the algorithm 

   Different sampling devices and different distances from the scene will cause differences in point cloud density. Existing methods for estimating point cloud density include distance-based methods and block-based methods. The distance-based average distance density representation method is to estimate the distribution density of point clouds by calculating the average distance of each point in the point cloud. The distance of a point is generally the distance between a point in the point cloud and the point closest to the point in the point cloud. In a point cloud with a number of points, the distance between a point and any other point is expressed, and the minimum distance between a point and other points is expressed. Then the average distance density of the point cloud is: the smaller the average distance, the denser the point cloud distribution, and the greater the density; the larger, the sparser the point cloud distribution, and the smaller the density. Therefore, it is feasible to estimate the point cloud density by the average distance. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574431763
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574431763
  ```  
 ![avatar]( 7a906a0b351d4b3aa338ec7490003581.png) 



--------------------------------------------------------------------------------

#  First, the main function 

##  1. AABB bounding box 

 1, get_axis_aligned_bounding_box () to get the aabb bounding box. 2, aabb.color = (1, 0, 0) to color the aabb bounding box. 3, get_center () returns the center of the geometric coordinates. 

###  1.1 Get the side length of the bounding box 

 4. get_extent () Gets the range/length of the bounding box in the x, y, and z dimensions. 5. get_geometry_type () Returns one of the registered geometric types. 6. get_half_extent () Returns half the range of the bounding box. 7. get_max_bound () Returns the maximum boundary of the geometric coordinates. 8. get_min_bound () Returns the minimum boundary of the geometric coordinates. 9. get_box_points () Returns the 8 points that define the bounding box. 

##  2. OBB bounding box 

 1, get_oriented_bounding_box () to get the obb bounding box. 2, obb.color = (0, 1, 0) to color the obb bounding box. 3, get_center () returns the center of the geometric coordinates. 

###  2.1 Get the side length of the bounding box 

 4. get_max_bound () returns the maximum boundary of the geometric coordinates. 5. get_min_bound () returns the minimum boundary of the geometric coordinates. 6. get_box_points () returns the 8 points that define the bounding box. 7. get_point_indices_within_bounding_box (self, points) returns the index to the points inside the bounding box. 

#  Code implementation 

 1. AABB bounding box 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744332
  ```  
 2. OBB bounding box 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744332
  ```  
#  III. Display of results 

 ![avatar]( 202102021955236.png) 

 1. AABB bounding box  

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744332
  ```  
 ![avatar]( 20210202195340630.png) 

 2. OBB bounding box  

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744332
  ```  


--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Calculation formula 

   The center of mass refers to the center of mass, which is considered an imaginary point where the mass of an object is concentrated at this point. Usually the coordinates of the center of mass of an object   

##  3. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574448173
  ```  
##  4. Function source code 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574448173
  ```  
#  Second, call function implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574448173
  ```  
#  Third, numpy implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574448173
  ```  
#  IV. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574448173
  ```  
 ![avatar]( b54112ac060a4be0b3efe7ef56dffabd.png) 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  I. Overview of algorithms 

   There is a point cloud and I want to find its maximum and minimum values on the three axes x, y, and z. 

##  1. Main function 

 Calculate the maximum value of point cloud coordinates 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574445078
  ```  
 Calculate the minimum value of point cloud coordinates 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574445078
  ```  
##  2. Function source code 

 Calculate the maximum value of point cloud coordinates 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574445078
  ```  
 Calculate the minimum value of point cloud coordinates 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574445078
  ```  
#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574445078
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574445078
  ```  
 ![avatar]( 203f4cab88b8443fb9ad3a09fdf8c34a.png) 

#  IV. Python Process Edition 

 Open3D Computing Point Cloud Coordinate Maximum (Python Procedural Edition) 



--------------------------------------------------------------------------------

#  I. Overview of algorithms 

   There is a point cloud and I want to find its maximum and minimum values on the three axes x, y, and z. 

##  1. Main function 

   The min () and amin () functions in numpy can be used to obtain the minimum value. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466296
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466296
  ```  
   When the input is not necessarily numpy.array, use np.amin (), if the input is np.array, you can directly use input.min (axis = n) to find the minimum value. Only the usage of np.min () and np.amin () is different. The result is the same. 

 How to use: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466296
  ```  
   The max () and amax () functions in numpy can be used to obtain the maximum value. The usage is the same as min () and amin (). 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466296
  ```  
#  III. Display of results 

 ![avatar]( 0ba18f0039024bd4855814878dff3ec0.png) 

 Python calculation results C++ calculation results, the results are exactly the same. 

#  C++ version code 

 PCL Calculation Point Cloud Axial Maximum 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

#  Roughness 

   Find the feature in the menu bar'Tools > Other > Roughness'. 

 ![avatar]( 17a91136f4284090be6bb85430d67834.png) 

  This tool can estimate the "roughness" of point clouds. 

 ![avatar]( 97eb795d96234f0e8d6ffa5ea57fed65.png) 

   Select one or a few point clouds and launch the tool. CloudCompare will only ask for "kernel size": the radius of the sphere centered on each point (see note below). Note: 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574451325
  ```  
#  III. Display of results 

 ![avatar]( 0b7011f7f51f4282bd39901818e53bcd.png) 



--------------------------------------------------------------------------------

#  I. Overview of algorithms 

##  1. Main function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574480640
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574480640
  ```  
##  2. Algorithm improvement 

   The example code of the official website needs to define a json file. For the implementation of the internal writing content of the json file, see: Open3D cropping points in any specified area 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574480640
  ```  
#  III. Display of results 

##  1. Primitive point cloud 

 ![avatar]( 20201120155609485.png) 

##  2. The cropped point cloud 

 ![avatar]( 20201120155618201.png) 

#  IV. Data download 

 Open3D cropping point cloud data test set Crop.rar 

#  CloudCompare 

 [1] CloudCompare——获取指定区域的点 



--------------------------------------------------------------------------------

#  First, the algorithm flow 

   Curvature downsampling means that the greater the curvature of the point cloud, the more sampling points. A simple and effective curvature downsampling method is as follows: 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574465059
  ```  
#  III. Display of results 

 ![avatar]( 20210303213455960.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574465059
  ```  


--------------------------------------------------------------------------------

#  Function overview 

   There are < cloud_viewer > for simple visualization operations and < pcl_visualizer > for advanced visualization in PCL, and there are also draw_geometries () and Visualizer () for visualization of point clouds in open3d. Personal understanding draw_geometries () in open3d is similar to < cloud_viewer > in PCL, but it is richer than < cloud_viewer > in PCL; Visualizer () in open3d is similar to < pcl_visualizer in PCL and cv :: s h ow () in opencv, which can realize all the functions in visualization operations. 

#  Second, the main function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466529
  ```  
 Set the background color from 0 to 1. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466529
  ```  
 Sets the size of the midpoint of the visual display. 

#  III. Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574466529
  ```  
#  IV. Display of results 

 ![avatar]( 8c62ad95edf34b5b99115448b2cd9a28.png) 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Implementation process 

   The RGB-D camera can measure the depth of each pixel. After measuring the depth, the RGB-D camera usually completes the pairing between the depth depth and the color map according to the placement of each camera during production, and outputs the one-to-one corresponding color map and depth map. We can read the color information and distance information at the same position, calculate the 3D camera coordinates of the pixels, and generate a point cloud. The calculation formula is: in the formula, it is the depth value, and the unit is meters; it is the scaling multiple of the depth value; it is the pixel coordinate, which is the 3D point cloud coordinate corresponding to the pixel; it is the focal length of the camera, and it is the optical center of the camera, which is the so-called internal parameter. The pose of the camera is also called the external parameter of the camera, which will change with the camera movement. Knowing the inner parameter can generate a point cloud from the color map and depth map, and knowing the outer parameter can splice the point cloud generated by the color map and depth map measured at different positions of the same object into a complete ground object point cloud. 

##  2. Main functions 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 Realize the fusion of color images and depth images into RGBD to generate point clouds. This function has 5 built-in parameters, which are: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 This function is used to set the internal parameters of the camera and can be used as follows: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 PinholeCameraIntrinsicParameters. PrimeSenseDefaul provides default camera parameters for Open3D. Its image resolution is: 640x480, focal length = (525.0, 525.0), optical center = (319.5, 239.5). The default external parameter is the identity matrix. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 This function implements the internal parameter setting of the camera. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 or 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 Note: The reason why the default outer parameter is reset to the above form is that the coordinates of the point cloud calculated in Open3D are all negative, see Equation 1; when using the identity matrix as the default outer parameter, the obtained point cloud is the opposite of the real scene. Multiplying the outer parameter set as above can remove the negative sign to make the point cloud consistent with the real scene. (As for why the above form? Try it yourself) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
 This function converts an RGBD image into a point cloud. 

#  Code implementation 

##  1. Experimental data 

 ![avatar]( 839b3ff8779f467fad42ed6f1eaa96f9.png) 

   The test data in the code is one of the case data provided in the "Fourteen Lectures on Visual SLAM" widely circulated on the Internet. Color image, depth image  

##  2. Main parameters 

 The resolution of the image is: 640x480, that is: width = 640, height = 480. The internal parameters of the camera are:. The external parameters of the camera are: -0.228993 0.00645704 0.0287837 -0.0004327 -0.113131 -0.0326832 0.993042 The external parameters are expressed using quaternions, the first three are translation parameters, and the last four are quaternion coefficients. 

##  3. Complete code 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574461462
  ```  
#  III. Display of results 

 ![avatar]( 9a58d0f421c94eb3a54037829c41069a.png) 

 1. Color image and depth image 2. Generated color point cloud 3. Generated colorless (intensity) point cloud  

#  IV. Relevant links 

 [1] 世界坐标系,相机坐标系和图像坐标系的转换(Python) [2] Open3D从RGB图与depth图产生RGB-D点云（采坑记录） [3] Open3d学习计划——6（RGBD图像） [4] Open3D 四元数、欧拉角、旋转向量转旋转矩阵 [5] Open3D 点云变换 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Overview of the principle 

   Equal spacing thinning algorithm: Set the sampling spacing in the original point cloud data to, first select 1 point at the beginning of the data; then keep 1 point per interval until all points are screened. The advantages of the equal spacing thinning method are simple, fast and efficient, but the disadvantage is that it cannot better retain the micro-terrain features. 

##  2. References 

>  [1] Wang Daojie, Chen Bei, Sun Jianhui. Influence of airborne LiDAR point cloud density on DEM accuracy [J]. Bulletin of Surveying and Mapping, 2022 (05): 140-144 + 169. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957449087
  ```  
#  III. Display of results 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957449087
  ```  
 ![avatar]( cb10f6fcd94c44c9a80ca34eed0cea61.png) 



--------------------------------------------------------------------------------

##  First, the main function 

 [1] Detailed explanation of the usage of numpy.where () [2] np.where () [0] and np.where () [1] The point cloud data source point cloud and the target point cloud are used in the code. From the figure, you can intuitively see the overlapping and non-overlapping parts of the two point clouds. The following code implements the extraction of overlapping and non-overlapping parts. 

##  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574488863
  ```  
##  III. Display of results 

 ![avatar]( 20210309100853851.png) 

##  IV. Reference link 

 [1] PCL 提取两片点云的重叠部分并保存 [2] PCL 提取两片点云的非重叠部分 



--------------------------------------------------------------------------------

#  Function overview 

##   1. Main function 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744101
  ```  
 select_by_index () in Open3D uses a binary mask to output only selected or unselected points. 

##   2. Source code 

 The source code is written in C++ and is very simple. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744101
  ```  
##   3. How to use 

   select_by_index () in Open3D currently only supports extracting subsets from point clouds. Where the data in the index should be formatted like this: [1, 2, 3, 4, 5, 6, 7, 8, 6, 6666, 4444,] So if you want to read the index of the point cloud to be extracted from a txt file, you need the following code to read and convert the data to the above format. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744101
  ```  
 1. Append () is used to add a new object at the end of the list. Syntax list.append (obj) where: list: list object; obj: object added to the end of the list. Note: The append () function has no return value, but will modify the original list. 2. Line.split () means to read the data by row and slice the string by specifying the delimiter. 

#  II. Complete code 

##   1. Read the index to extract the point cloud 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744101
  ```  
##   2. Application in the algorithm 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744101
 ```python
def display_inlier_outlier(cloud, m_ind):

    inlier_cloud = cloud.select_by_index(m_ind)

    outlier_cloud = cloud.select_by_index(m_ind, invert=True)

    print("Showing outlier_cloud (red) and inlier_cloud (green): ")

    outlier_cloud.paint_uniform_color([1, 0, 0])

    inlier_cloud.paint_uniform_color([0, 1, 0])

    o3d.visualization.draw_geometries([inlier_cloud, outlier_cloud],

                                      window_name = "Inner and Outer Points",

                                      width=1024, height=768,

                                      left=50, top=50,

                                      mesh_show_back_face=False)

  ```  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 20240203095744101


--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Remarks 

>  Detailed algorithm introduction can be viewed in the original text: Zhou Q Y, Park J, Koltun V. Fast Global Registration [J] .2016. and point cloud matching algorithm, paper sharing Fast Global Registration, Fast Global Registration. 

##   2. References 

>  The following two papers are improvements to the algorithm [1] Shen Changjiang, Wu Yundong, Cai Guorong, Chen Shuili. Lidar point cloud registration method for multi-view buildings based on quaternary constraints [J]. Journal of Jimei University (Natural Science Edition), 2019, 24 (05): 393-400. [2] Shen Changjiang. Research on multi-view Lidar point cloud registration technology based on tuple constraints [D]. Jimei University, 2019. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574441504
  ```  
#  III. Display of results 

 ![avatar]( 20210112163514570.png) 

#  IV. Reference link 

 [1] Global registration 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Overview of the principle 

 ![avatar]( 55d2f4a5ec6c4f6e83282a61605b6f8e.png) 

   As shown in Figure a, if the angle between the normal vector of the point cloud in the local area is large, it is a non-flat area; on the contrary, if the angle between the normal vector does not change much as shown in Figure b, the area is relatively flat. Therefore, define the arithmetic average of the angle between a point cloud and its neighbor normal vector: In the formula, it is the angle between the point cloud and the neighborhood normal vector. Point pi is a non-characteristic point. 

##  2. References 

>  [1] Han Yifei, Yang Ziqian, Zheng Fu, Wang Yanqiu, Sun Zhibin. Improved point cloud registration algorithm based on FPFH and normal vector [J/OL]. Semiconductor Optoelectronics: 1-6 [2021-08-28]. https://doi.org/10.16818/j.issn1001-5868.2021.04.001. [2] Song Chenghang, Li Jinru, Liu Guanjie. Improved ICP algorithm point cloud registration method using feature point sampling consistency [J]. Beijing Surveying and Mapping, 2021 (03): 317-322. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574484195
  ```  
#  III. Display of results 

 ![avatar]( aa443a357944419b9b694fe116590df6.png) 



--------------------------------------------------------------------------------

#  First, the principle of the algorithm 

##  1. Algorithm overview 

   Farthest Point Sampling (FPS): As the name suggests, the point farthest from the previously sampled points is selected for each sample. It can better ensure that the sampled points have good coverage, so it is widely used in the field of point cloud segmentation (e.g., PointNet ++, PointCNN, PointConv, PointWeb). However, the computational complexity of FPS is that the amount of computation is square related to the number of points in the input point cloud. This suggests that FPS may not be suitable for processing large-scale point clouds. For example, when entering a large field attraction cloud with millions of points, it takes up to 200 seconds to downsample it to 10% of the original size using FPS. 

##  2. Implementation process 

##  3. References 

>  [1] Hu Q , Yang B , Xie L , et al. RandLA-Net: Efficient Semantic Segmentation of Large-Scale Point Clouds[J]. 2019. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574426173
  ```  
#  III. Display of results 

 ![avatar]( 20210608073858440.png) 

 Before filtering: 85 points. After filtering: 43 points.  

#  IV. Reference link 

 [1]《三维点云处理》学习笔记（2）：滤波器 [2] 200倍的提速！华人博士生提出大场景三维点云语义分割新框架 [3] 三维点云处理：5滤波：降采样 [4] PCA降维、法向量估计、点云体素及FPS滤波 



--------------------------------------------------------------------------------

#  I. Overview of algorithms 

   Given a specified elevation value, get all points in the point cloud data with the same elevation. 

#  Code implementation 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574497008
  ```  
#  III. Display of results 

##  1. Primitive point cloud 

 ![avatar]( 47ff749d52d04d458bd249a40892c7c9.png) 

##  2. Get the results 

 ![avatar]( 236f639a3e944d0db1724aff1bc14d41.png) 

#  IV. Experimental data 

 [1] 常用经典斯坦福点云数据 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

