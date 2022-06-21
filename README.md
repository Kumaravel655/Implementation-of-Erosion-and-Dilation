### Ex.No:10
### DATE: 
# <p align="center">Implementation-of-Erosion-and-Dilation</p>
# 
## Aim
To implement Erosion and Dilation using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV

## Algorithm:
### Step 1:
Import the necessary packages.
### Step 2:
Create the Text using cv2.putText
### Step 3:
Create the structuring element.
### Step 4:
Erode the image.
### Step 5:
Dilate the image.
 
 
 <br><br>
 <br><br>
 
## Program:
```
/*
Developed by   : Kumaravel V
Register Number: 212220230027
*/
```
``` Python
# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1=np.zeros((300,500),dtype='uint8')
font=cv2.FONT_ITALIC=3
img2=cv2.putText(img1,"Kumaran",(5,70),font,3,(255),5,cv2.LINE_AA)
cv2.imshow("Original",img2)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Create the structuring element
kernel1=np.ones((5,5),np.uint8)

# Erode the image
erode=cv2.erode(img2,kernel1)
cv2.imshow("Erosion1",erode)
cv2.waitKey(0)
cv2.destroyAllWindows()

# Dilate the image
dilute=cv2.dilate(img2,kernel2)
cv2.imshow("Dilution",dilute)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

 
 
  <br><br><br><br> 
 
 <br><br>
 <br><br>
## Output:

### Display the input Image
![Screenshot (148)](https://user-images.githubusercontent.com/75235334/170829153-cd03325e-2899-4875-9d8e-8521a419bf87.png)
### <br><br>Display the Eroded Image
 ![Screenshot (149)](https://user-images.githubusercontent.com/75235334/170829163-2ab57684-fe21-4900-b791-a65c25999ea9.png)

### Display the Dilated Image
 ![Screenshot (150)](https://user-images.githubusercontent.com/75235334/170829169-0bfc7938-ba6b-4d53-8b88-b5347fccd375.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
