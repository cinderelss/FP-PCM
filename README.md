# Image Noise Filtering Project

This project focuses on applying image noise filtering techniques, including the addition of noise (Salt and Pepper noise) and noise removal using Median and Gaussian filters. The Python implementation showcases the process of loading an image, introducing noise, and applying filters to improve image quality.

---

## Overview
The project implements image filtering techniques to mitigate noise. Specifically, it:
- Adds Salt and Pepper noise to a grayscale image.
- Removes noise using a Median Filter and a Gaussian Blur.

The implementation includes:
- A `SaltAndPaper` function to simulate noise.
- A `median_filter` function for noise removal.
- A `gaussian_blur` function leveraging a custom convolution implementation.

---

## Dataset
The project uses a grayscale image file named `mild.jpg` located in the working directory. Replace this with any desired grayscale image for testing.

---

## Code Explanation

### Salt and Pepper Noise
The `SaltAndPaper` function introduces Salt and Pepper noise to an image by randomly assigning pixel values to 0 (black) or 255 (white) with a specified density.

```python
def SaltAndPaper(image, density):
    # Parameters:
    # image: Input grayscale image
    # density: Noise density (0-1)
```

### Median Filter
The `median_filter` function applies a median filter to the noisy image. This filter replaces each pixel value with the median of its surrounding pixels, effectively removing noise.

```python
def median_filter(data, filter_size):
    # Parameters:
    # data: Input image
    # filter_size: Size of the filter window (e.g., 3x3, 5x5)
```

### Gaussian Blur
The `gaussian_blur` function applies a Gaussian blur using a custom convolution operation. The Gaussian kernel is generated using the `gaussian_kernel` function.

```python
def gaussian_blur(image, kernel_size):
    # Parameters:
    # image: Input image
    # kernel_size: Size of the Gaussian kernel
```

---

## How to Run the Code
1. Place the grayscale image (`mild.jpg`) in the working directory.
2. Run the script in Python.

---

## Results
The output consists of:
1. The original image.
2. The noisy image (Salt and Pepper noise added).
3. Denoised images after applying:
   - A Median Filter (3x3 and 5x5).
   - Gaussian Blur (3x3).

---

## Conclusion
This project demonstrates how to simulate image noise and remove it using filtering techniques. The Median Filter effectively handles Salt and Pepper noise, while Gaussian Blur smoothens the image, reducing noise artifacts.

These techniques are fundamental in image preprocessing and have wide applications in computer vision and image analysis.

---


