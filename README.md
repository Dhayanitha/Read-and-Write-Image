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
### Developed By: H.Dhayanitha
### Register Number: 212220230010
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('pic6.jpg',1)
cv2.imshow('colorimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image

```
cv2.imwrite('sunset.jpg',color_image)
cv2.imshow('sunset',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
iii) #Find the shape of the Image
```
import cv2
color_image=cv2.imread('pic6.jpg',-1)
print(color_image.shape)

```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('pic6.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
        cv2.imshow('212220230010, H.Dhayanitha',color_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
v) #To cut and paste portion of image
```
cut=color_image[260:280,100:300]
color_image[60:80,100:300]=cut
cv2.imshow('slicedimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image

![pic6](https://user-images.githubusercontent.com/75235032/161386747-6ea10ca7-46e4-401a-946a-63c57c156bd1.jpg)

### ii)Write the image

![sunset](https://user-images.githubusercontent.com/75235032/161386774-d7cf03ed-1d5e-4e57-a834-140c9956c78c.jpg)

### iii)Shape of the Image

![code 1](https://user-images.githubusercontent.com/75235032/161386793-2dedaf93-ebe8-4c50-b708-92154526be42.jpg)

### iv)Access rows and columns

![rows_coloums](https://user-images.githubusercontent.com/75235032/161386811-b8181412-bac6-4fbe-a50f-5199fff90fdb.jpg)

### v)Cut and paste portion of image

![sliced_img](https://user-images.githubusercontent.com/75235032/161386826-c369efbb-8ea0-4f8d-891f-2754a2e70749.jpg)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


