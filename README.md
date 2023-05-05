Download Link: https://assignmentchef.com/product/solved-cse578-assignment1-camera-calibration
<br>



<strong>Assignment-1 </strong>

<strong>Instructions:</strong>

<ul>

 <li>The goal of the assignment is to familiarize you to the process of camera calibration and the critical role it plays in using any measurements of the world from images.</li>

 <li><strong>Make sure that the assignment that you submit is your own work. Any breach of this rule could result in serious actions including an F grade in the course.</strong></li>

 <li>The experiments and report writing takes time. Start your work early and do not wait till the deadline.</li>

 <li>Make sure your files can be opened. Corrupted files will not be entertained.</li>

 <li>You can use C/C++, Python or Matlab for this. However, you are expected to implement it yourselves and not use an existing implementation.</li>

</ul>

<strong>Tasks:</strong>

This assignment requires you to implement and compare the two camera calibration techniques. We would also like to test the quality of the parameters estimated from these calibration methods. You are expected to do the following:

<h1>Direct Linear Transform</h1>

<ol>

 <li>For the given image <em>calib-object.jpg </em>using any 20-30 different points on different planes and perform the Direct Linear Transform (DLT) based calibration as discussed in class. Report the projection matrix, camera matrix, rotation matrix and projection center. Note that you need to manually estimate the image co-ordinates of the given world points and refer to <em>calib-object-legend.jpg </em>for world measurements. Each chessblock is 28X28 mm.</li>

 <li>Implement the RANSAC based variant of the above calibration method and report your observations.</li>

 <li>Repeat the above experiments after correcting for radial distortion. Estimate the radial distortion parameters from the straight lines in the image. What do you observe regarding the resulting parameters?</li>

</ol>

CV (CSE/ECE 578)                        Assignment 1 – Page 2 of 2            Posted: 29 January 2020

<h1>Zhangs Method</h1>

<ol>

 <li>Use checkerboard images <em>JPG – IMG5470.JPG </em>and perform camera calibration using Zhang’s Method. You can use the available OpenCV or Matlab implementation.</li>

 <li>Using the estimated camera parameters compute the image points and overlay a wireframe over the actual image of chessboard using straight lines between the computed points. Refer to <em>example-wireframe.png </em>for reference. What do you observe about the overlay? <strong>Note that do not use the image points found using the cvFindChessboardCorners for wireframe overlay. Size of each square on checkerboard 29mmX29mm</strong></li>

 <li>What is the image of the world origin, given the calibration matrix? Does this result bear out in your observations?</li>

</ol>

<h1>Hands on</h1>

Select a camera that you would like to use for the assignments. Note that you might be using this camera for future assignments also.

<ol>

 <li>Perform the above calibration methods using the images taken by your camera. Use the calibration object for which you can measure the world co-ordinates for DLT and printed checkerboard pattern for Zhangs Method.</li>

 <li>Vary the focus of your phone and comment on the results.</li>

</ol>

Write a detailed report of your findings and results as mentioned in the previous steps, and submit it as a pdf file. You should also include your code and images that you acquired for the experiments at the end of the pdf file.