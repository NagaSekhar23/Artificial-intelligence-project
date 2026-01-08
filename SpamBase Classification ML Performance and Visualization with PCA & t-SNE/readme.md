# SpamBase Classification: ML Performance and Visualization with PCA & t-SNE

This project explores the classification of spam emails using the well-known **SpamBase dataset**. It evaluates the performance of standard machine learning (ML) methods and investigates the impact of dimensionality reduction techniques—specifically **Principal Component Analysis (PCA)** and **t-Distributed Stochastic Neighbor Embedding (t-SNE)**—on model accuracy and data visualization.

## Project Overview

- **Objective**: Classify emails as spam or non-spam using traditional ML models.
- **Key Techniques**:
  - Standard ML classifiers (e.g., Logistic Regression, SVM, Random Forest)
  - Dimensionality reduction via PCA and t-SNE
  - Visualization of high-dimensional data in 2D using PCA and t-SNE
- **Findings**:
  - Standard ML methods achieve good performance on the SpamBase dataset.
  - PCA simplifies the data but may reduce model accuracy.
  - t-SNE provides better visualization of class separation, aiding in understanding the dataset structure.

## Results

- **Model Accuracy**: Evaluated using standard ML pipelines.
- **Visualizations**:
  - Left: 2D PCA projection
  - Right: 2D t-SNE projection  
  *(See notebook figures for details)*

## Tools & Libraries

- Python
- Scikit-learn (for ML and dimensionality reduction)
- Matplotlib & Seaborn (for visualization)
- Jupyter Notebook (for interactive analysis)

## Repository Structure
