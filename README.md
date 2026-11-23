# WORKSHOP-3 Canny Edge Detection using OpenCV
## Author
## NAME : SAI PRAVEEN C
## REG.NO : 212225230239

## Overview :

This project demonstrates the implementation of the Canny Edge Detection algorithm using Python and OpenCV. Canny Edge Detection is a widely used image processing technique for identifying object boundaries and significant intensity changes in an image.

## License

This project is licensed under the MIT License.

## Objectives :

- Load and process a sample image.
- Convert the image to grayscale.
- Apply the Canny Edge Detection algorithm.
- Visualize and analyze the detected edges.
- Study the impact of different threshold parameters on edge detection results.

## Technologies Used :

- Python
- OpenCV
- NumPy
- Matplotlib
- Jupyter Notebook


## Algorithm :

1. Read the input image.
2. Convert the image to grayscale.
3. Apply Gaussian filtering to reduce noise.
4. Compute image gradients.
5. Perform non-maximum suppression.
6. Apply double thresholding.
7. Track edges using hysteresis.
8. Display the detected edges.


## Applications :

- Object Detection
- Image Segmentation
- Medical Image Analysis
- Autonomous Vehicles
- Computer Vision Systems
- Pattern Recognition

## Requirements :

```bash
pip install opencv-python numpy matplotlib
```

## Running the Project:

1. Clone the repository:

```bash
git clone https://github.com/your-username/canny-edge-detection-opencv.git
```

2. Open Jupyter Notebook:

```bash
jupyter notebook
```

3. Run:

```bash
CANNY EDGE DETECTION.ipynb
```

## PROGRAM :

```
import cv2
import matplotlib.pyplot as plt
```

```
img = cv2.imread('sai1.jpeg',cv2.IMREAD_GRAYSCALE)
blurred =cv2.GaussianBlur(img, (5,5),0)
edges = cv2.Canny(blurred, 50, 150) 
```

```
plt.figure(figsize=(10,5))
plt.subplot(121),plt.imshow(img, cmap='gray')
plt.title('Original Image'), plt.axis('off')
plt.subplot(122),plt.imshow(edges, cmap='gray')
plt.title('Detected Edges'), plt.axis('off')
plt.show()
```

## OUTPUT :

<img width="807" height="467" alt="image" src="https://github.com/user-attachments/assets/4d2f7b14-66c7-4b7f-bb4d-b37a9e44371e" />

## RESULT:

The Canny Edge Detection algorithm effectively detects object boundaries and important image features. The quality of edge detection depends on the selected threshold values, making parameter tuning an essential part of image processing applications.
