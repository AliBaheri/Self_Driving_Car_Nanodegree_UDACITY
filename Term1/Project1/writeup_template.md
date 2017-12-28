# **Finding Lane Lines on the Road** 

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline.

 - Gaussian Smoothing
 
 - Canny edges detection: The CED algorithm is employed to extract the edges of the Gaussian Smoothing image. I have tried a 
   few values for high and low threshold to finalize these parameters.
 
 - Masked edges region of interest: Next, I mask the ROE for identifying the lane lines.
 
 - Hough transform: Finally Hough transform is applied on the edges detection of the image.


### 2. Identify potential shortcomings with your current pipeline


My pipeline is not robust with "challeng" task. I am still trying to find a systematic approach to tune various parameters in my pipeline.


### 3. Suggest possible improvements to your pipeline

One possible improvement for the current pipeline is modifying the region of interest (ROE). My plan is to write a function to find ROE in a systematic fashion. 

