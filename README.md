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
![Reading](https://user-images.githubusercontent.com/94827772/160898237-e27db2e9-3f56-4bba-a4a4-4e5e7460afb0.png)

### ii)Write the image
![Writing](https://user-images.githubusercontent.com/94827772/160898339-74189789-3d79-47d4-8fcd-a2e1179e238f.png)

### iii)Shape of the Image
![Shape](https://user-images.githubusercontent.com/94827772/160898376-e7a45d73-7485-4185-a5c5-3269f64d471f.png)

### iv)Access rows and columns
![AccRows colms](https://user-images.githubusercontent.com/94827772/160898414-6707590d-2785-4b90-83df-900792d98295.png)


### v)Cut and paste portion of image
![Accessing](https://user-images.githubusercontent.com/94827772/160898433-0a14380b-324d-49ef-9644-ef0f2fcf3766.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


