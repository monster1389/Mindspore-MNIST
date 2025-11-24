# MindSpore MNIST Handwritten Digit Recognition

## 📋 Project Overview

This project implements a handwritten digit recognition system using Huawei's MindSpore deep learning framework. The model is trained on the classic MNIST dataset to classify handwritten digits (0-9) with high accuracy. For the fking homework of our institute. 

## 🚀 Features

- **Simple CNN Architecture**: Uses a convolutional neural network (LeNet5) optimized for MNIST
- **MindSpore Framework**: Built with Huawei's MindSpore deep learning platform
- **High Accuracy**: Achieves &gt;98% accuracy on test dataset
- **Easy to Use**: Simple training scripts
- **Cross-platform**: Supports CPU, GPU, and Ascend devices

## 📦 Requirements

### Environment Setup
- win11
- Python 3.7+
- MindSpore 2.0+
- NumPy
- Matplotlib

### Installation
```bash
# Install MindSpore (choose based on your device)
# For CPU
pip install mindspore

# For GPU
pip install mindspore-gpu

# For Ascend (NPU)
pip install mindspore-ascend

# Install other dependencies
pip install numpy matplotlib
