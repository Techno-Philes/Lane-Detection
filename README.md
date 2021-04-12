# Open-CV-Lane-Detection

**Problem Statement:**

A lane detection car *can easily detect lanes* and can travel anywhere a normal car does. Explorations in AI and Deep Learning have made such innovations possible with essential training. Lane detection is the primary and the most important step in the deployment of an autonomous car.

## **Steps involved in Lane Detection:**
  - Reading the image. If reading a video convert into frames.
  - Conversion of the image into GRAY scale
  - Using filter or Gaussian blur to get a clear image
  - Detect the edges using Canny function
  - Create a mask for the Canny Image
  - Identify the coordinates of the lane
  - Fit the detected coordinates into the Canny Image
  - Lane detection is completed.

## Gist about Coding:

  - **1.	Reading the Image/Video:**
    - In case of a video, we first capture the video by using the *VideoCapture( )* function. From this we use the *.read( )* function to get each and every frame.
  -  **2.	Conversion of the Image into GRAY scale:**
    - The frame that we have are in *BGR* (Blue, Green, Red). Now we convert this to a gray scale using *cv2.cvtColor( )* function by passing the method cv2.COLOR_BGR2GRAY.  
  - **3.	Using filter or Gaussian blue to get a clear image:**
    - In order to reduce the noise or blur in the frame we use the “*.filter( )*” or “*.Gaussianblur( )*” function.
  - **4.	Detect the edges using Canny function:**
    - The “*.Canny( )” function can be used to detect all the edges in the frame.
  - **5.	Identify the coordinates of the lane:**
    - Now we detect the dimensions of the road lane and a mask is created which is of the same dimensions as the frame using the “*.mask( )*”. The *bitwise AND* function is then used between the canny image and the mask.

# Comprehending The Code!!

**The following explanation of code works only for the given images and videos, depending upon the region of interest.**

_To perform lane detection the Libraries used are:_
- Opencv
- Numpy
- matplotlib.pyplot
