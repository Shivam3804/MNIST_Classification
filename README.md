# MNIST Digit Classification

This project involves building and comparing two neural network models for classifying handwritten digits using the MNIST dataset.

## Overview

The MNIST dataset is a benchmark dataset consisting of 70,000 grayscale images of handwritten digits (0–9), each of size 28x28 pixels. The goal is to train the two models and evaluate them.

## Models Implemented

### 1. Fully Connected Neural Network (Dense Only)
- **Architecture**: Flatten → Dense(128, ReLU) → Dense(10, Softmax)
- **Test Accuracy**: **~96.91%**

### 2. Convolutional Neural Network (CNN)
- **Architecture**:  
  Conv2D(32, 3x3, ReLU) → MaxPooling2D(2x2) →  
  Conv2D(64, 3x3, ReLU) → MaxPooling2D(2x2) →  
  Flatten → Dense(64, ReLU) → Dense(10, Softmax)
- **Test Accuracy**: **~98.20%**

## Technologies Used
- Python
- TensorFlow / Keras
- Jupyter Notebook / Google Colab

## Key Learnings
- Understanding of image data preprocessing.
- Comparison of fully connected vs. convolutional architectures.
- Experience with TensorFlow model design, training, and evaluation.

## Results Summary

| Model                  | Test Accuracy |
|------------------------|---------------|
| Dense Only             | ~96.91%       |
| CNN (with Conv2D)      | ~98.20%       |
