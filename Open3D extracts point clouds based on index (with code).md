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
