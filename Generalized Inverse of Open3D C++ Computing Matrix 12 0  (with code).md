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

