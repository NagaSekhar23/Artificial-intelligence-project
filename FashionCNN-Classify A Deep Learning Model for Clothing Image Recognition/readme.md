# FashionCNN-Classify: Clothing Image Recognition with Deep Learning

A deep learning project using a Convolutional Neural Network (CNN) to classify fashion items from the FashionMNIST dataset. This repository demonstrates training, validation, and testing of a custom CNN model for image classification tasks.

## 📌 Project Overview

This project implements a simple yet effective CNN architecture to classify 10 types of clothing items (e.g., T-shirts, trousers, dresses, shoes) from grayscale images. The model is trained using PyTorch and evaluated on the FashionMNIST dataset, which is a popular benchmark for image classification.

### Key Features:
- **Model Architecture**: Custom CNN with two convolutional layers and two fully connected layers.
- **Dataset**: FashionMNIST (10 classes of clothing items).
- **Training Metrics**: Accuracy on training, validation, and test sets.
- **Environment**: Runs on CPU (can be adapted for GPU).

---

## 🧪 Results

| Metric       | Value          |
|--------------|----------------|
| Train Accuracy | 94.19%         |
| Validation Accuracy | 88.87%       |
| Test Accuracy  | 88.61%         |

**Model Configuration:**
- Random Seed: 2024
- Learning Rate: 0.01
- Batch Size: 64
- Model: `FashionCNN`

---

## 🛠️ Model Architecture

The CNN consists of:
1. **Feature Extractor**:
   - Two convolutional layers (`Conv2d`) with ReLU activation.
   - Max pooling layers for spatial down-sampling.
2. **Classifier**:
   - Fully connected layers (`Linear`) for classification.
   - Final output layer with 10 units (one for each clothing class).

```python
FashionCNN(
  (features): Sequential(
    (0): Conv2d(1, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
    (1): ReLU()
    (2): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
    (3): Conv2d(32, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1))
    (4): ReLU()
    (5): MaxPool2d(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
  )
  (classifier): Sequential(
    (0): Linear(in_features=3136, out_features=128, bias=True)
    (1): ReLU()
    (2): Linear(in_features=128, out_features=10, bias=True)
  )
)
