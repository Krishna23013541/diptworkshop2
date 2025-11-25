# WORKSHOP-3--Canny-Edge-Detection
# NAME: KRISHNA KUMAR R
# REG NO: 212223230107
# PROGRAM:

```

import cv2
import matplotlib.pyplot as plt
img = cv2.imread('krishh.jpg',cv2.IMREAD_GRAYSCALE)
blurred =cv2.GaussianBlur(img, (5,5),0)
edges = cv2.Canny(blurred, 50, 150) 
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()

```


# OUTPUT:
<img width="945" height="524" alt="image" src="https://github.com/user-attachments/assets/8ec63bd5-a82b-4e37-bf2e-86255dee2775" />

