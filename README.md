# Implementation-of-Erosion-and-Dilation
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

## Output:

### Display the input Image
![Screenshot (148)](https://user-images.githubusercontent.com/75235334/170828874-c31146ac-441b-44ba-8d09-11833f6b61a0.png)

### <br><br>Display the Eroded Image

![Screenshot (149)](https://user-images.githubusercontent.com/75235334/170828911-f9471a09-fd4d-468c-a771-a981585e30a4.png)


### Display the Dilated Image
![Screenshot (150)](https://user-images.githubusercontent.com/75235334/170828954-c25cd7ec-5703-4080-a71f-9ba01c2670ee.png)

## <br><br><br><br><br><br><br><br>Result
Thus the generated text image is eroded and dilated using python and OpenCV.
