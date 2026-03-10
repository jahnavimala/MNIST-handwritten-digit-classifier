# MNIST-handwritten-digit-classifier
A machine learning project implementing a classification algorithm  Convolutional Neural Network (CNN/SVM) to recognize handwritten digits (0-9) using the classic Yann LeCun MNIST dataset.

# Handwritten Digit Recognition (MNIST)

## Project Overview
This repository contains a machine learning model capable of recognizing handwritten digits. While trained on the MNIST dataset, the goal is to provide a pipeline that can process images of digits written on physical paper.

## Dataset
- **Source:** [MNIST Database](http://yann.lecun.com/exdb/mnist/)
- **Details:** 70,000 grayscale images of digits (0-9).
- **Format:** 28x28 pixels.

## Features
- **Data Augmentation:** Techniques used to handle different writing styles and rotations.
- **Normalization:** Scaling pixel values from [0, 255] to [0, 1].
- **Model Architecture:** [Insert your model, e.g., 2D Convolutional Neural Network].

## Image Processing Pipeline
To recognize digits from an actual piece of paper:
1. **Grayscale Conversion**: Removing color noise.
2. **Gaussian Blur**: Reducing detail to focus on the shape of the stroke.
3. **Thresholding**: Converting the image to pure black and white (Binary).
4. **Contour Detection**: Finding the bounding box of the digit to crop it.
5. **Resizing**: Scaling the crop to 28x28 pixels to match the MNIST training data.
