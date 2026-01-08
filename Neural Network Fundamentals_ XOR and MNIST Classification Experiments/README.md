# Neural Network Fundamentals: XOR and MNIST Classification

This repository contains two Jupyter Notebook assignments that explore foundational concepts in neural networks using PyTorch.

## Overview

- **Assignment 3 - Problem 2.ipynb**  
  Demonstrates why the XOR problem is not linearly separable and how a simple Multi-Layer Perceptron (MLP) with a hidden layer and non-linear activation can solve it perfectly.

- **Assignment 3 - Problem 1.ipynb**  
  Implements a flexible MLP for image classification on both the classic handwritten digits MNIST and Fashion-MNIST datasets, with support for different activations, optimizers, and performance visualization.

## Assignment 3 - Problem 2: Solving XOR with MLPs

### Key Concepts
- Why XOR cannot be solved by a single linear classifier (not linearly separable)
- How a hidden layer with non-linear activation (Tanh or ReLU) transforms the feature space to make XOR solvable
- Effect of hidden layer size (H = 1 → insufficient capacity; H = 4/8 → sufficient)
- Impact of input noise on decision boundaries and generalization
- Comparison between Tanh and ReLU activations

### Highlights
- Generates a noisy XOR dataset (200 extra points around the four corners)
- Trains a small MLP (2 → 4 → 1) with Tanh activation
- Achieves ~97–100% accuracy on train/validation
- Plots training and validation loss curves

## Assignment 3 - Problem 1: MLP on MNIST & Fashion-MNIST

### Features
- Customizable `MLP` class supporting multiple hidden layers and activations (ReLU, Sigmoid, Tanh, LeakyReLU)
- Training/evaluation functions with automatic GPU support (CUDA if available)
- Data loading for:
  - Classic MNIST (from `mnist.pkl`)
  - Fashion-MNIST (via `torchvision`)
- Training loop includes:
  - Optimizer selection (Adam, SGD, Adagrad)
  - Tracking of train/validation accuracy
  - Automatic saving of the best model (highest validation accuracy)
- Visualizations:
  - Train vs. validation accuracy curves
  - Test set confusion matrix (Seaborn heatmap)

### Example Results (Fashion-MNIST)
- Architecture: 784 → 128 → 64 → 10 (ReLU)
- Optimizer: Adam (lr = 0.001)
- Test accuracy: ~88–90% (typical range)
##pip install torch torchvision matplotlib seaborn numpy scikit-learn

## Requirements

```bash
Python >= 3.8
torch
torchvision
matplotlib
seaborn
numpy
scikit-learn


##pip install torch torchvision matplotlib seaborn numpy scikit-learn
