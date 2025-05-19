# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary pacakages
<br>

### Step2:
Create the text using cv2.putText
<br>

### Step3:
Create the structuring element
<br>

### Step4:
Erode the image
<br>

### Step5:
Dilate the Image
<br>

 
## Program:
```
NAME : VIGNESH V
REG NO : 212223230241
```
# Import the necessary packages
```
import cv2
import numpy as np
from matplotlib import pyplot as plt
```
# Create the Text using cv2.putText
```
# Load the image
img1=np.zeros((100,700),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the text using cv2.putText
cv2.putText(img1,'VIGNESH V' ,(5,70),font,4,(255),2,cv2.LINE_AA)
```
# Create the structuring element
```
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(5,5))
```
# Erode the image
```
img_dilate=cv2.dilate(img1,kernel1)
img_erode=cv2.erode(img1,kernel1)
```
# Dilate the image
```
plt.figure(figsize=(12, 5))
plt.subplot(1,3,1)
plt.imshow(img1,cmap='gray')
plt.subplot(1,3,2)
plt.imshow(img_dilate,cmap='gray')
plt.subplot(1,3,3)
plt.imshow(img_erode,cmap='gray')
```
## Output:

### Display the input Image
<br>
<br>
<br>

![Screenshot 2025-05-19 184913](https://github.com/user-attachments/assets/aa444865-3760-43e8-b8c7-89de17dfcb38)


<br>
<br>

### Display the Eroded Image
<br>
<br>
<br>

![Screenshot 2025-05-19 184931](https://github.com/user-attachments/assets/79ff88cf-b182-4a4a-854b-954b7031dee6)

<br>
<br>

### Display the Dilated Image
<br>
<br>
<br>

![Screenshot 2025-05-19 184944](https://github.com/user-attachments/assets/01864c8c-9382-42e1-b3fa-f9a9888f8344)

<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
