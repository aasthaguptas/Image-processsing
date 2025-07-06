# Image-processsing
It captures your image and allows yoou to edit it

!pip install opencv-python

import cv2
import numpy as np
import matplotlib.pyplot as plt

img=cv2.imread(r"C:\Users\HP\OneDrive\Pictures\Camera Roll\dd.jpg")

print(type(img))

cv2.imshow("bootcamp",img)
cv2.waitKey(0)
cv2.destroyAllWinmdows()

print(img.shape)

img_resize=cv2.resize(img,(203,300))

cv2.imshow("bootcamp",img_resize)
cv2.waitKey(0)
cv2.destroyAllWinmdows()

(img_resizprinte.shape)

cv2_imshow(img_resize)//google colab

img_flip=cv2.flip(img,0)

cv2.imshow("flipped Image",img_flip)
cv2.waitKey(0)
cv2.destroyAllWinmdows()

img_crop=img[100:300,200:500]

cv2.imshow("Cropped Image",img_crop)
cv2.waitKey(0)
cv2.destroyAllWinmdows()

cv2.imwrite(r"croppedImg16.jpg",img_crop)
