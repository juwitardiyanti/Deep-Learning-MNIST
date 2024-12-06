# MNIST CNN Model with TensorFlow/Keras

This project demonstrates how to train a Convolutional Neural Network (CNN) to classify handwritten digits from the MNIST dataset using TensorFlow and Keras.

## Project Overview

The project involves the following steps:
1. Loading and preprocessing the MNIST dataset.
2. Defining a CNN architecture for image classification.
3. Training the model with training data and validating with a split of the training set.
4. Visualizing training results including loss and accuracy.

## Requirements

Install the required libraries:

- `tensorflow`
- `matplotlib`

To install these dependencies, run:

```bash
pip install tensorflow matplotlib
```

## Dataset

The MNIST dataset is a collection of 70,000 grayscale images of handwritten digits (0-9), each of size 28x28 pixels. The dataset is divided into:
- 60,000 training samples
- 10,000 testing samples

The dataset is included in TensorFlow and can be loaded directly.

## Model Architecture

The CNN model includes:
- Two convolutional layers followed by max-pooling and dropout for feature extraction.
- A fully connected dense layer with ReLU activation for high-level representation.
- A final output layer with softmax activation for classification into 10 classes.

## Training Configuration

- Optimizer: Adam
- Loss Function: Categorical Cross-Entropy
- Metrics: Accuracy
- Epochs: 50
- Batch Size: 100
- Validation Split: 20%
