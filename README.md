# WORKSHOP-3-Canny-Edge-Detection

# Name : Thirisha A
# Reg No : 212223040228


# CODE :
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('3sha.jpeg',cv2.IMREAD_GRAYSCALE)
# Apply Gaussian blur to reduce noise
blurred =cv2.GaussianBlur(img, (5,5),0)
# Detect edges using Canny
edges = cv2.Canny(blurred, 50, 150) #Adjust threshold values as needed
# Plot the original image and the detected edges
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()

```
# OUTPUT :

<img width="691" height="395" alt="image" src="https://github.com/user-attachments/assets/3fe9e54d-29b0-4208-9ec6-bfc290b2f135" />

