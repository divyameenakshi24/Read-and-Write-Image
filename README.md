# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

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
### Developed By: A.Divya Meenakshi
### Register Number: 212220230014
i) #To Read,display the image
```
  import cv2
  import random
  col=cv2.imread("cute.jpg",1)
  cv2.imshow("col",col)
  cv2.waitKey(0)

```
ii)GREY IMAGE
```
gray=cv2.imread("cute.jpg",0)
cv2.imshow("gray",gray)
cv2.waitKey(0
```
iii) #To write the image
```

cv2.imwrite("dicon.jpg",gray)

```
iv) #Find the shape of the Image
```
print(col.shape)


```
v) #To access rows and columns

```
import random
for i in range(100):
    for j in range(col.shape[1]):
        col[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow("col",col)
cv2.waitKey(0)



```
vi) #To cut and paste portion of image
```
color=cv2.imread("fates.jpg",1)
tag=color[300:400,300:400]
color[50:150,50:150]=tag
cv2.imshow("color",color)
cv2.waitKey(0)



```

## Output:

### i) Read and display the image

<br>
![img](https://user-images.githubusercontent.com/75235402/161681333-c665fd76-73ef-4456-ae5b-c8bca28120c7.JPG)

<br>

### ii)Grey image

<br>
![img 2](https://user-images.githubusercontent.com/75235402/161681386-bab48132-0e20-4c43-b45c-85ab68e28058.JPG)

<br>

### iii)Write the image

<br>

![img 3](https://user-images.githubusercontent.com/75235402/161681559-57e14292-0852-4832-8fc6-2330f16fd441.JPG)


<br>

### iv)Shape of the Image

<br>
![img 4](https://user-images.githubusercontent.com/75235402/161681585-6984402b-b9f0-46df-9ee9-2d46d8d9a493.JPG)


<br>

### v)Access rows and columns
<br>
![img 5](https://user-images.githubusercontent.com/75235402/161681650-bd5ae221-f9f3-4eda-9389-1a798e6823d4.JPG)


<br>

### vi)Cut and paste portion of image
<br>
![img 6](https://user-images.githubusercontent.com/75235402/161681662-9bc4c947-7673-497d-a24d-a3a83f25e7aa.JPG)


<br>,

## Result:
Thus the images are read, displayed, and written successfully using the python program.


