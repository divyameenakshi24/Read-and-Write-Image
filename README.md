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

![img](https://user-images.githubusercontent.com/75235402/161933216-c7cf4320-d951-4400-8691-66df2705ec2f.jpg)

<br>

### ii)Grey image

<br>

![img 2](https://user-images.githubusercontent.com/75235402/161933284-efdd65dd-64ad-4034-b462-750b10328502.jpg)
<br>


### iii)Write the image

<br>

![img 3](https://user-images.githubusercontent.com/75235402/161933697-08307719-4681-4421-93b1-3d12ddc05656.jpg)



<br>

### iv)Shape of the Image

<br>
![img 4](https://user-images.githubusercontent.com/75235402/161933757-f6c842c1-9997-480d-91ed-6c32f7261783.jpg)


<br>

### v)Access rows and columns
<br>


![img 5](https://user-images.githubusercontent.com/75235402/161933811-ddc0c90a-91f8-4e72-80a9-d590d20dccc5.jpg)

<br>

### vi)Cut and paste portion of image
<br>
![img 6](https://user-images.githubusercontent.com/75235402/161933921-762e90e2-e9fc-4ed5-9b0c-ffbc084663c0.jpg)


<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


