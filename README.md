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
```

## 📁 Project Structure

```
├── README.md                 # This file
├── test.py                   # Training script
├── requirements.txt          # Python dependencies
└── MNIST_Data/               # Dataset
```

## 🎯 Quick Start

1. Data Preparation
bash
```
# Download MNIST dataset
pip install download

%env no_proxy='a.test.com,127.0.0.1,2.2.2.2'
from download import download

url = "https://mindspore-website.obs.cn-north-4.myhuaweicloud.com/" \
      "notebook/datasets/MNIST_Data.zip"
path = download(url, "./", kind="zip", replace=True)
```
2. Training
bash
```
# Train the model
python test.py
```


## 🏗️ Model Architecture

The model uses a simple but effective CNN architecture:

```
Input (28×28×1)
    ↓
Conv2D (32 filters, 5×5)
    ↓
ReLU + MaxPool (2×2)
    ↓
Conv2D (64 filters, 5×5)
    ↓
ReLU + MaxPool (2×2)
    ↓
Flatten
    ↓
Dense (1024 units)
    ↓
ReLU + Dropout
    ↓
Dense (10 units) → Output
```
