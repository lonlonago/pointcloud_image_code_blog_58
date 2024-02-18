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

