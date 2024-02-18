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

