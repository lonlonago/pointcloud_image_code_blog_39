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

