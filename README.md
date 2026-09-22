# NAME: YOGAMAHENDRAN G
# REG NO:212225040500



# Aim
To write a Python program using OpenCV to perform morphological operations such as Erosion and Dilation on an image.

# The program performs the following operations:

Image Erosion

Image Dilation

Software Used

Anaconda – Python 3.7

Jupyter Notebook / VS Code

OpenCV (cv2)

NumPy

Matplotlib

# Algorithm
Step 1:
Import the required libraries: OpenCV, NumPy, and Matplotlib.

Step 2:
Create a blank image using NumPy.

Step 3:
Insert text onto the image using OpenCV's text drawing function.

Step 4:
Display the original image.

Step 5:
Create a structuring element (kernel) of suitable size.

Step 6: Image Erosion
Apply the erosion operation using the created kernel.
Remove pixels from the boundaries of foreground objects.
Display the eroded image.

Step 7: Image Dilation
Apply the dilation operation using the same kernel.
Add pixels to the boundaries of foreground objects.
Display the dilated image.

Step 8:
Compare the original, eroded, and dilated images.

# Program
# Developed By
# Name:Yogamahendran g

# Register No: 212225040500


```

import cv2
import matplotlib.pyplot as plt
img = cv2.imread("nature.jpeg")
plt.imshow(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
plt.title("Original Image")
plt.axis("off")
plt.show

```


<img width="915" height="565" alt="639263379-bb2bfa3a-f9e4-488e-86e2-98db4e25f69a" src="https://github.com/user-attachments/assets/82d07e2f-5659-43a5-9b1c-21125302dbab" />

```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
erosion = cv2.erode(img, kernel, iterations=1)
plt.imshow(erosion, cmap="gray")
plt.title("Image Erosion")
plt.axis("off")
plt.show()

```



<img width="915" height="570" alt="639263510-09d2c823-8779-4a8d-8240-49cf7b97782d" src="https://github.com/user-attachments/assets/cfd434bc-9cce-4299-a7ed-d18875716a2f" />

```
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
dilation = cv2.dilate(img, kernel, iterations=1)
plt.imshow(dilation, cmap="gray")
plt.title("Image Dilation")
plt.axis("off")
plt.show()

```


<img width="891" height="560" alt="639263676-3ef0765d-c324-4679-a4b2-a78adf1b0ffb" src="https://github.com/user-attachments/assets/86b20e1e-5f1b-49be-8127-bcde67b8477b" />

# Result
Thus, the morphological operations Erosion and Dilation are successfully implemented using OpenCV.
