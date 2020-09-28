# **Finding Lane Lines on the Road** 


**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

I modified draw_lines(). It consists of 3-steps. First, points are classified by the left lane or right lane according to the slope of (x1, y1) and (x2, y2). Second, By using the np.polyfit, classified points are fitting to the first-order polynomial. Lastly, vertices are connected by coefficients which are generated in second step.

### 2. Identify potential shortcomings with your current pipeline

Sometimes, it has poor quality when a specific scene of the video. The performance highly depends on calibration parameters


### 3. Suggest possible improvements to your pipeline

If I generate the lanes based on cubic polynomials, I think it will have more smooth lanes

