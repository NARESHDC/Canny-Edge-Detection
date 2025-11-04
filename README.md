# WORKSHOP-3-Canny-Edge-Detection

# Name : NARESH.M
# Reg No : 212223220064


# CODE :
```
import cv2
import matplotlib.pyplot as plt
# Read the image
img = cv2.imread('melkin.jpg',cv2.IMREAD_GRAYSCALE)
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
<img width="1720" height="895" alt="{9B1D2E77-3B78-4033-A5C6-A7FA02FEFDA4}" src="https://github.com/user-attachments/assets/d3e11685-be04-4494-a8a8-64aff3781868" />
