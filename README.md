##  First, the principle of the algorithm 

###  1. Overview of the principle 

  The registration accuracy of the point cloud adopts the root mean square error RMSE. The smaller the root mean square error, the higher the registration accuracy; the degree of overlap is to calculate the proportion of the nearest neighbor pairs to all points. The larger the degree of overlap, the better the registration effect. See the algorithm source code for the specific calculation process. 

###  2. Algorithm source code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596953
 ```  
###  3. Main functions 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596953
 ```  
This function is used to evaluate the registration between point clouds. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596953
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574596953
 ```  


--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  Different sampling devices and different distances from the scene will cause differences in point cloud density. Existing methods for estimating point cloud density include distance-based methods and block-based methods. The distance-based average distance density representation method is to estimate the distribution density of point clouds by calculating the average distance of each point in the point cloud. The distance of a point is generally the distance between a point in the point cloud and the point closest to the point in the point cloud. In a point cloud with a number of points, the distance between a point and any other point is expressed, and the minimum distance between a point and other points is expressed. Then the average distance density of the point cloud is: the smaller the average distance, the denser the point cloud distribution, and the greater the density; the larger, the sparser the point cloud distribution, and the smaller the density. Therefore, it is feasible to estimate the point cloud density by the average distance. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574575024
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574575024
 ```  
##  IV. Relevant links 

Usage of accumulated in C++ 



--------------------------------------------------------------------------------

##  Centroid 

  The centroid of a face is the geometric center of a cross-sectional figure. The centroid is for a physical body, while the centroid is for abstract geometry. For a physical body of uniform density, the centroid and centroid coincide. The geometric center or centroid of an object in dimensional space is the intersection of all hyperplanes that divide into two equal parts of the moment. Informally, it is the average of all points in it. If the mass of an object is evenly distributed, the centroid is the center of gravity. - Baidu Encyclopedia 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555077
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555077
 ```  


--------------------------------------------------------------------------------

##  I. Overview of algorithms 

  The Chamfer Distance distance can calculate the average shortest point distance between the generated point cloud data and the labeled point cloud data. Open3D can be directly used to calculate the Chamfer Distance distance of the point cloud. For more details on the application of the Chamfer Distance in point clouds, please refer to: PCL calculation of point cloud chamfer distance (Chamfer Distance) or master's thesis: [1] Zhang Yonghan. Research on monocular vision 3D point cloud reconstruction technology based on deep learning [D]. Northeast Electric Power University, 2020. I won't go into too much detail here. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574599430
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574599430
 ```  
![avatar]( 7efab6c58174488595dbf46a99b54229.png) 



--------------------------------------------------------------------------------

##  First, the result preview 

  The red is the query point, and the green is the point in its cylindrical neighborhood. 

![avatar]( 34a1e5ca12d245ce995ee5fc916c7595.png) 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574587403
 ```  
##  III. Display of results 

![avatar]( 39d78c3082f642068845701d7a87a756.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Generalized inverse 

   Non-square matrices do not have inverses, but there are generalized inverses (pseudo-inverses). For a matrix, if there is a matrix such that: Then it is the generalized inverse of. Generalized inverses that satisfy the above four formulas are unique. With the following singular decomposition: where, is a diagonal matrix, the diagonal elements are singular values. Then the generalized inverse can be written as:  

###  2. Calculation process 

1. First, the matrix is decomposed by SVD to obtain three matrices, which are column matrices, which are the singular values of the matrix arranged from top to bottom and from large to small. 2. If the number of elements in the matrix is the original matrix, the original matrix has a singular value. Build a matrix of size V.col () * U.col (), where each element of the previous diagonal of the matrix is each singular value, that is, the reciprocal of each element of the matrix. It should be noted that the elements of the matrix are non-negative, and the order is reversed from large to small. 3. Finally, use the formula to construct the pseudo-inverse matrix of the matrix. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574519999
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574519999
 ```  
##  IV. Reference link 

[1] 利用Eigen求广义逆矩阵 [2] C++SVD分解求伪逆 （Eigen库）（附C++代码） 



--------------------------------------------------------------------------------

##  I. Overview 

  Calculating the maximum distance between points in the same point cloud is an important step in the overlap estimation in the 4PCS registration algorithm, and is the basis for realizing handwritten 4PCS and improving it. To this end, the Open3D implementation is used to obtain the maximum distance in a given point cloud set, and return the minimum and maximum coordinate points 

###  1. References 

>  [1] Wang Fei, Liu Rufei, Ren Hongwei, Chai Yongning. Multi-phase vehicle laser point cloud registration using road target characteristics [J]. Journal of Surveying and Mapping Science and Technology, 2020, 37 (05): 496-502. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574579573
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574579573
 ```  


--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  Calculate the mean and standard deviation of each field of the given point cloud data x, y, z coordinates, where the standard deviation is implemented as n-1. 

##  Second, the main function 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574519608
 ```  
  Given a vector of type float, calculate the mean and standard deviation of the given point cloud data simultaneously, where the standard deviation is n-1 

##  III. Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574519608
 ```  
##  IV. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574519608
 ```  


--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Calculation formula 

  Calculate the normalized 3x3 covariance matrix and centroid for a given set of points. Normalization means that each item in the matrix is divided by the number of valid point clouds. For a small number of points, or if explicit sample variance is required, use the scaled covariance matrix, where the number of points used to calculate the covariance matrix is used. The formula is: where is the point in the point cloud, is the centroid of the point cloud. 

###  2. Main functions 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581358
 ```  
###  3. Function source code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581358
 ```  
##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581358
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574581358
 ```  


--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

![avatar]( 77f1c90ddfe945f788f3dfa7355affd8.png) 

See: PCL point cloud boundary extraction 

##  Code implementation 

BoundaryEstimation.h 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574549820
 ```  
BoundaryEstimation.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574549820
 ```  
BEmain.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574549820
 ```  
##  III. Display of results 

![avatar]( 92f37d32b493403885afe669067adf1c.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Overview of the principle 

![avatar]( 31f767b23c5c442492e9a189b8361399.png) 

###  2. References 

>  LIU Ke. Research on Boundary Extraction Algorithm of Planar Point Cloud [D]. Changsha University of Science and Technology, 2017. 

##  Code implementation 

AlphaShape.h 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563045
 ```  
AlphaShape.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563045
 ```  
main.cpp 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563045
 ```  
##  III. Display of results 

![avatar]( 06ed4011c097408aa17f6bfaa9793836.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###   1. Overview of the principle 

   Alpha-shape is a generalization of the convex hull algorithm. One can intuitively think of alpha-shape as follows: Imagine a large piece of ice cream containing dots of S chocolate chunks. Using one of these spherical ice cream spoons, we can cut out all the parts of the ice cream chunks, and we can dig holes inside without touching the chocolate chunks (e.g., parts that cannot be reached by just moving the spoon from the outside). We end up with a (not necessarily convex) object, which consists of vertices, arcs, and points. If we now straighten all the round faces into triangles and line segments, we can visually describe the so-called alpha shape. 

###   2. Function analysis 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538570
 ```  
Implementing this method in Open3D requires attention to the following two points: 

###   3. References 

>  [1] H.Edelsbrunner and D. G. Kirkpatrick and R. Seidel: On the shape of a set of points in the plane, IEEE Transactions on Information Theory, 29 (4): 551–559, 1983 [2]Alpha shapes 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574538570
 ```  
##  III. Display of results 

![avatar]( 8aeed7dfcc994123869de8b33e35dc42.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Axial angle representation 

![avatar]( 03b04926e3c94739b5b5b35a0add7416.png) 

   Assuming that the rigid body coordinate system is the rotation angle of B (Oxyz) about the axis represented by the unit vector, its corresponding rotation matrix can be deduced. First, assume that the axis of the rigid body coordinate system B coincides with any axis represented, and then the rotation angle of the B coordinate system around the Z axis of the reference coordinate system A (OXYZ) is such that the projection of the axis in the XOY plane coincides with the X axis, and then around the angle, the z axis and the Z axis coincide, and then around the Z axis rotation angle. Finally, in order to make z return to the position coinciding with the axis, the rotation angle around the Y axis and the rotation angle around the Z axis can be used, as shown in the figure below.  

###  2. Rodriguez formula 

![avatar]( 8be0bb3ac7c5433eac680f4d0cd4b3b8.png) 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574533871
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574533871
 ```  
##  IV. Relevant links 

[1] Open3D(C++) 根据向量做点云旋转 [2] Open3D(C++) 计算向量的夹角 [3] Open3D(C++) 角度制与弧度制的相互转换 [4] Open3D (C++) 点云变换 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

###  1. Projection density theory and method 

![avatar]( 288f96df99374c7bbc708ec89f39a5f8.png) 

    The 3-dimensional coordinate points are directly projected vertically onto the horizontal plane or the value is taken as an arbitrary constant to count and calculate the number of projection points contained at any position on the horizontal plane as (Density of Projected Points). In an ideal state (the target surface is smooth, unobstructed, and all sampling points are valid points), the value is related to the height of the target, the vertical distance from the center of the scanner to the target, and the spatial resolution of the scanner. To simplify the calculation, the measurement area can be divided into regular grids, the grid is uniformly numbered, and the number of projected points on each grid unit is counted and this value is used as the value of the grid unit. This way, the value can be expressed discretely. Values have the following characteristics:  

1. On the ground, the value is relatively uniform and relatively small as a whole; 2. At the boundary of the building (the gray area in the figure), the value is much larger than that of other areas and forms a continuous band; 3. Inside the building, if the noise is removed, the impact value is 0; 4. Independent point-like features, such as lamp posts, have larger local values and smaller surrounding values; 5. Block-like features, such as trees and cars, are locally larger and occupy a certain area. When the grid area increases to a certain value, the block-like features have the same characteristics as the independent point-like features. Using the above characteristics and selecting a reasonable threshold, the point cloud can be divided according to the following formula:  

###  2. References 

>  Shi Wen, Li Bijun, Li Qingquan. Image segmentation method of vehicle laser scanning distance based on projection point density [J]. Chinese Journal of Surveying and Mapping, 2005 (02): 95-100. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574555954
 ```  
##  III. Display of results 

![avatar]( 4e42e7f9a3e144248b46905691cd4a1d.png) 

 Original point cloud, extract the result  



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  In the building point cloud, there is obvious difference between the normal vector of the elevation point and the normal vector of the plane point, and the segmentation of the elevation point and the plane point can be realized by setting the corresponding threshold according to the component of the normal vector in the Z direction. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586984
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574586984
 ```  
![avatar]( 1e10297534e74f31813081e133c69374.png) 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  For a vector, the angle included in the vector is:   

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574536056
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574536056
 ```  


--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  Given,,, three points, the sign of the directed area of the three points is determined in the following way: Imagine that you are standing at a point in the plane, facing. You walk to, if to your right (then we say that the three vectors are arranged "clockwise"), the sign of the area is negative, otherwise positive. If the three points are adjacent, the area is zero. Using this signed area, you can get the regular unsigned area (as the absolute value of the signed area), and you can also determine whether the points are arranged clockwise or counterclockwise in a specified order (useful in convex hull algorithms, for example). 

###  1. Method 1 

  Utilize the theorem that the determinant of a matrix is equal to the signed area of the parallelogram spanned by the column (or row) vectors of that matrix. This is similar to the definition of the cross product in two dimensions. By dividing this area by 2, the area of the triangle can be obtained. Using the determinant of the sum as the column vector, the directed area can be obtained. 

###  2. Method 2 

  According to Helen's formula, the determinant of a triangle twice the area is: if the area is positive, it is expressed on the left side of the directed line segment. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574525323
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574525323
 ```  
##  IV. Reference link 

[1] 三角形的定向（符号）面积 



--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  The equation for the point direction of a straight line is: where, the direction vector, the known point. The formula for the distance from a point outside the line to the line is:  

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577199
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574577199
 ```  


--------------------------------------------------------------------------------

##  First, the principle of the algorithm 

  The formula for calculating a point outside the plane to the plane is: 

Detailed derivation process see: point to plane distance. 

##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563830
 ```  
##  III. Display of results 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574563830
 ```  


--------------------------------------------------------------------------------

##  Introduction to the algorithm 

###  1. Overview 

  First, use K-nearest neighbor search to find the nearest neighbor of each point, then calculate the Euclidean distance from each point to the nearest neighbor, and finally color render according to the distance. 

###  2. Main functions 

  ComputeNearestNeighborDistance function in Open3D calculates the Euclidean distance from each point to its nearest neighbor. 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574528788
 ```  
###  3. Algorithm source code 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574528788
 ```  
##  Code implementation 

 ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574528788
 ```  
##  III. Display of results 

![avatar]( 437ab8d03993426b8a14948ec5132106.png) 



--------------------------------------------------------------------------------

