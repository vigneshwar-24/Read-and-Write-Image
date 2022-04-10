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
### Developed By:Vingneshwar S
### Register Number: 212220230058
i) #To Read,display the image
```
import cv2
image_1=cv2.imread("img1.jpg")
image_2=cv2.imread("img2.jpg")
cv2.imshow("pic1",image_1)
cv2.waitKey(0)
cv2.imshow("pic2",image_2)
cv2.waitKey(0)


```
ii) #To write the image
```
cv2.imwrite("pic_1.jpg",image_1)
cv2.imwrite("pic_2.jpg",image_2)


```
iii) #Find the shape of the Image
```python3
print(image_1.shape)
print(image_2.shape)


```
iv) #To access rows and columns

```python3
for i in range(70,90):
    for j in range(110,170):
        image_2[i][j]=[0,0,0]
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)



```
v) #To cut and paste portion of image
```python3
image_1[200:220,110:175]=image_1[70:90,110:175]
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image

<br>![Screenshot (29)](https://user-images.githubusercontent.com/77089276/162615669-9272f503-b28b-42a7-9fd1-5753a106bf17.png)
![Screenshot (30)](https://user-images.githubusercontent.com/77089276/162615683-c43c0898-77f5-4fe0-9494-af376e4f594a.png)

<br>

### ii)Write the image

<br>![Screenshot (36)](https://user-images.githubusercontent.com/77089276/162615687-97178f58-e325-4336-8d94-e8bce6e78f0b.png)

<br>

### iii)Shape of the Image

<br>![Screenshot (35)](https://user-images.githubusercontent.com/77089276/162615694-08986729-c15f-45e3-98bd-3589b271cf0c.png)

<br>

### iv)Access rows and columns
<br>![Screenshot (32)](https://user-images.githubusercontent.com/77089276/162615699-d3a61277-534b-4b31-81a1-fbb0ffbb3fde.png)

<br>

### v)Cut and paste portion of image
<br>![Screenshot (33)](https://user-images.githubusercontent.com/77089276/162615700-6c8a97a1-8eb6-4a95-9272-2d0d7fea5dad.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.


