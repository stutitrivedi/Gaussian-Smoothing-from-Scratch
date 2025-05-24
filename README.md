# Gaussian Smoothing from Scratch
 Gaussian Smoothing from Scratch

This project implements a custom Gaussian smoothing (blurring) algorithm in Python. Gaussian smoothing is a foundational technique in image processing used to reduce image noise and detail, making it easier to detect general shapes and patterns in images.

Problem Statement:

Images captured from real-world environments often contain high-frequency noise, which can obscure important features and distort object boundaries. Gaussian smoothing reduces this noise by applying a Gaussian filter, which smoothens pixel intensity variations in a natural and visually pleasing way.

Solution Overview:

A Gaussian kernel generator and convolution function implemented manually using NumPy.

A function that applies the Gaussian filter to an image based on specified kernel size and sigma (standard deviation).

A demonstration using a sample image to visualize the smoothing effect.

A comparison with the result produced by OpenCV's built-in cv2.GaussianBlur() function.

An optional version using separable 1D kernels for computational efficiency (extra credit).

Note: This project does not use OpenCV functions such as cv2.getGaussianKernel(), cv2.GaussianBlur(), cv2.filter2D(), or cv2.sepFilter2D() in the custom logic. These functions are used only for comparison.

Project Structure

gaussian-smoothing/

custom_gaussian.py : Python script with the custom implementation

compare_with_opencv.py : Script to compare custom output with OpenCV output

GaussianSmoothing.ipynb : Jupyter notebook version with detailed explanation and visualization

example_image.jpg : Sample image used for testing


How It Works

Generate a 2D Gaussian kernel based on the given kernel size and sigma.

Normalize the kernel so that the sum of all elements is 1.

Perform 2D convolution of the kernel with the input image manually using nested loops.

Return the smoothed image as output.

(Optional) Use separable 1D kernels (horizontal and vertical) to reduce computational cost.


Requirements

Python 3.x

numpy

opencv-python

matplotlib
