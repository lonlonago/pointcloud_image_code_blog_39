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
