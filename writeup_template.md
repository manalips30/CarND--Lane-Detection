

                              **Finding Lane Lines on the Road**

Pipeline Design:
1. Input Image -> RGB to Gray conversion 
2. region Selection 
3. Edge Extraction using Canny edge detection  
4.  Apply Hough Transform -> Lines 
5. Separate lines into positive and negative slopes and fit lines for each to get continuous lane representation 
6. Annotate original image with continuous line


  


 







 Potential shortcomings with current pipeline


1. One potential shortcoming would be what would happen when the brightness of image will vary continuously. 

2. Another shortcoming could be due to curved lane lines as the current approach is based on the slope of the lane lines.


   Possible improvements to pipeline:


1. A possible improvement would be using HSV transform efficiently so that detection will be consistent regardless of brightness.


2. Another potential improvement could be to use cache memory to save previous data regarding lane lines and extrapolate accordingly or using Kalman filter to predict future data .





