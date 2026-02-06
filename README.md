# CNN from Scratch: Fashion MNIST Classification

This repository contains a professional implementation of a **Convolutional Neural Network (CNN)** built entirely from scratch using **NumPy** and **Pandas**. The project focuses on the manual implementation of spatial feature extraction and the mathematical backpropagation of gradients through non-linear layers.

## Technical Highlights
Unlike standard implementations using high-level frameworks (TensorFlow/PyTorch), this project implements the "under-the-hood" logic:

* **Efficient Convolutions**: Implemented 2D convolutional layers using `numpy.lib.stride_tricks` and `sliding_window_view` to handle image patches efficiently.
* **Max Pooling**: Developed a pooling layer to reduce spatial dimensions and extract dominant features from the 28x28 grayscale images.
* **Weight Initialization**: Utilized **He Initialization** to maintain signal variance and prevent vanishing gradients in deep ReLU layers.
* **Manual Backpropagation**: Derived and implemented the chain rule for convolutional filters, allowing the model to learn spatial hierarchies.

## Results
The model achieves high performance on the Fashion MNIST dataset:
* **Training Accuracy**: Reached **~94%** within 10 epochs.
* **Validation Accuracy**: Consistently achieved **~89%** on unseen test data.

## Tech Stack
* **Language**: Python
* **Core Math**: NumPy, Pandas
* **Visualization**: Matplotlib
