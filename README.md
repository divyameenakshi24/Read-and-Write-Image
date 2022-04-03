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
https://user-images.githubusercontent.com/75235402/161443723-c96c3cc8-b452-4f92-bcd8-5b425d74b14f.JPG

<br>

### ii)Grey image

<br>
![img 2](https://user-images.githubusercontent.com/75235402/161443841-93679e24-ade3-46fd-813b-1bc5472b339e.JPG)

<br>

### iii)Write the image

<br>
![img 3](https://user-images.githubusercontent.com/75235402/161443741-9eb37048-22da-47d2-91d3-379a8d4d52bb.JPG)


<br>

### iv)Shape of the Image

<br>
![img 4](https://user-images.githubusercontent.com/75235402/161443752-338a146b-4057-4ff5-b826-605c112c2de7.JPG)

<br>

### v)Access rows and columns
<br>
![img 5](https://user-images.githubusercontent.com/75235402/161444276-213d35dd-5878-418d-9fbc-fae19b96406f.JPG)

<br>

### vi)Cut and paste portion of image
<br>
![img 6](https://user-images.githubusercontent.com/75235402/161444289-f23bbe4b-de46-4413-a879-f53069eb1644.JPG)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


