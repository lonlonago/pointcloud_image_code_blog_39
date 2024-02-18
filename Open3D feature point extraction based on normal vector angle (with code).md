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

