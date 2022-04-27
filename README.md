# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
 Convert BGR and RGB to HSV and GRAY

### Step2:
Convert HSV TO RGB AND BGR

### Step3:
Convert RGB and BGR to YCrCb

### Step4:
To Split and merge RGB Image

### Step5:
To Split and merge HSV Image

## Program:
```python
# Developed By: G.harish
# Register Number: 212220230021

# i) Convert BGR and RGB to HSV and GRAY
import cv2
img = cv2.imread('tony.jpg')
cv2.imshow('Original Image',img)
img1 = cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',img1)
img2 = cv2.cvtColor(img,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',img2)

img3 = cv2.cvtColor(img,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',img3)

img4 = cv2.cvtColor(img,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',img4)
cv2.waitKey(0)





# ii)Convert HSV to RGB and BGR
cv2.imshow('Original Image',img)

img5 = cv2.cvtColor(img,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',img5)
img6 = cv2.cvtColor(img,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV2RGB',img6)
cv2.waitKey(0)





# iii)Convert RGB and BGR to YCrCb
cv2.imshow('Original Image',img)

img7 = cv2.cvtColor(img,cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',img7)

img8 = cv2.cvtColor(img,cv2.COLOR_BGR2YCrCb)
cv2.imshow('RCB2YCrCb',img8)
cv2.waitKey(0)




# iv)Split and Merge RGB Image
red = img[:,:,0]
green = img[:,:,1]

blue = img[:,:,2]
img9=cv2.merge((blue,green,red))
cv2.imshow('Merged',img9)
cv2.waitKey(0)



# v) Split and merge HSV Image
hsv=cv2.cvtColor(img,cv2.COLOR_BGR2HSV)
cv2.imshow("ORIGINAL HSV_IMAGE",hsv)
h,s,v = cv2.split(hsv)
img10=cv2.merge((h,s,v))
cv2.imshow('Merged',img10)
cv2.waitKey(0)





```
## Output:
### i) BGR and RGB to HSV and GRAY

![harish exp3](https://user-images.githubusercontent.com/75246297/165573655-9b407f41-e536-4c66-b794-af71161f6a2f.jpg)


### ii) HSV to RGB and BGR
![harish exp3 1](https://user-images.githubusercontent.com/75246297/165573814-ba44ad6e-b3e4-4259-bd27-6c95d3088895.jpg)



### iii) RGB and BGR to YCrCb
![harish exp3 2](https://user-images.githubusercontent.com/75246297/165573941-1d727896-4a94-4bdd-88ba-7195a80a7418.jpg)



### iv) Split and merge RGB Image

![harish exp3 3](https://user-images.githubusercontent.com/75246297/165574100-88a8b961-62a9-432c-98ec-c282b0aa89b0.jpg)



### v) Split and merge HSV Image

![haish exp3 4](https://user-images.githubusercontent.com/75246297/165574463-d0e00aac-091b-4761-bb02-5d2eda19a4fa.jpg)




## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.

