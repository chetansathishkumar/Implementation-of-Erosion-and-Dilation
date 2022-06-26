## EX.NO: 10 <br>
## DATE: 28-05-2022
## <p align="center">IMPLEMENTATION OF EROSION AND DILATION</p>

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
<br>Import the necessary packages.


### Step2:
<br>Create the Text using cv2.putText.

### Step3:
<br>Create the structuring element.

### Step4:
<br>Erode and Dilate the image.

### Step5:
<br>End Program.

 
## Program:
```
DEVELOPED BY : P S Chetan
REG NO :212220230033
```

``` Python
# Import the necessary packages

import cv2
import numpy as np
import matplotlib.pyplot as plt



# Create the Text using cv2.putText
img1=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX
cv2.putText(img1,'Chetan',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.imshow(img1)


# Create the structuring element
kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))




# Erode the image

image_erode=cv2.erode(img1,kernel)
plt.imshow(image_erode)
plt.axis('off')
plt.title('Erosion')



# Dilate the image

image_dilate=cv2.dilate(img1,kernel)
plt.imshow(image_dilate)
plt.axis('off')
plt.title('Dilation')



```
## Output:

### Display the input Image
<br>![image](https://user-images.githubusercontent.com/75260837/171333119-3332d60c-0357-4e6b-b81a-b656a06d4752.png)

<br>
<br>
<br>
<br>
<br>

### Display the Eroded Image
<br>![image](https://user-images.githubusercontent.com/75260837/171333170-8df1e82d-3759-4c46-b9a0-c89615b60d82.png)

<br>
<br>
<br>
<br>
<br>

### Display the Dilated Image
<br>![image](https://user-images.githubusercontent.com/75260837/171333267-57413060-0c01-4220-9d33-6da1011ab285.png)

<br>
<br>
<br>
<br>
<br>
<br>

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
