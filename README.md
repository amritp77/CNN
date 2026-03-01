->Image Classification with Convolutional Neural Networks (CIFAR-10)

This repository contains a Jupyter Notebook that explores and compares different neural network architectures for image classification using the CIFAR-10 dataset. The main objective of this project is to analyze how architectural design influences model performance on small RGB images (32×32 pixels) belonging to ten distinct object categories.

-> Project Overview

The notebook implements and evaluates three different neural network approaches:

Fully Connected Neural Network (Baseline Model)

Serves as a reference model.

Flattens image pixels into a one-dimensional vector.

Demonstrates the limitations of ignoring spatial structure in image data.

Adapted AlexNet Architecture

Modified to handle smaller CIFAR-10 images.

Uses convolutional layers for feature extraction.

Includes ReLU activations, pooling layers, dropout, and normalization.

Adjusted kernel sizes and fully connected layers to suit 32×32 inputs.

Compact VGG-style Network (TinyVGG)

Inspired by VGG design principles.

Stacks small convolutional filters to capture hierarchical features.

Emphasizes depth and structured feature learning.

->Technical Implementation

The notebook is implemented using:

PyTorch for model building and training

Torchvision for dataset handling and preprocessing

Matplotlib for visualization

Scikit-learn for performance evaluation metrics

Data Preprocessing Includes:

Random cropping and horizontal flipping (data augmentation)

Channel-wise normalization

Batch loading using DataLoader

Device configuration for CPU/GPU support

-> Model Evaluation

Each architecture is trained and evaluated using:

Training and validation accuracy

Loss tracking

Classification reports

Confusion matrix visualization

Performance comparison across models

This allows a structured analysis of how convolutional feature extraction improves classification accuracy compared to fully connected networks.

-> Learning Objectives

This project demonstrates:

The importance of spatial feature extraction in image tasks

Differences between shallow and deep architectures

How architectural design impacts generalization

Practical implementation of CNN training pipelines

Model comparison using quantitative metrics

-> How to Use

Clone the repository

Install required dependencies (PyTorch, torchvision, sklearn, matplotlib)

Run the notebook step by step

Train and evaluate models

Observe performance differences between architectures
