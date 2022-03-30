# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.<br>
i) Read, display, and write an image.<br>
ii) Access the rows and columns in an image.<br>
iii) Cut and paste a small portion of the image.<br>

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
```python
# Developed By: G Venkata Pavan
# Register Number: 212221240013
# To Read,display the image

import cv2
color=cv2.imread('Bike2.jpg',1)
cv2.imshow('212221240013',color)
cv2.waitKey(0)


# To write the image

import cv2
color=cv2.imread('Bike2.jpg',1)
cv2.imwrite('Bike2.jpg',color)
cv2.waitKey(0)


# Find the shape of the Image

import cv2
color=cv2.imread('Bike2.jpg',1)
print(color.shape)


# To access rows and columns

import cv2
color=cv2.imread('Bike2.jpg',1)
import random
for i in range (100):
    for j in range(color.shape[1]):
        color[i][j] = [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212221240013-AccessingRowsAndColumns',color)
cv2.waitKey(0)


# To cut and paste portion of image:

import cv2
color=cv2.imread('Bike2.jpg',1)
tag = color[20:80,20:80]
color[90:150,90:150] = tag
cv2.imshow('212221240013-AccessingRowsAndColumns',color)
cv2.waitKey(0)

```
## Output:

### i) Read and display the image
<br>
![Reading](https://user-images.githubusercontent.com/94827772/160898060-1ee31c22-cc26-40c3-bbcd-fa28f9ee3c5a.png)

<br>
### ii)Write the image
<br>
![Writing](https://user-images.githubusercontent.com/94827772/160897417-76246c9c-cb54-46f4-91b1-73237c0d10de.png)
<br>

### iii)Shape of the Image
<br>
![Shape](https://user-images.githubusercontent.com/94827772/160897461-a3574db1-007d-4ee2-82c0-5ae16bfc8b6d.png)
<br>


### iv)Access rows and columns
<br>
![AccRows colms](https://user-images.githubusercontent.com/94827772/160897495-206bdc61-1328-4b60-b492-c9c28944e5a3.png)
<br>


### v)Cut and paste portion of image
<br>
![Accessing](https://user-images.githubusercontent.com/94827772/160897529-903fb9b8-06d8-49eb-9b23-bab5ef5baba9.png)
<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


