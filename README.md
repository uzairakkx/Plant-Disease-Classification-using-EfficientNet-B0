# Plant-Disease-Classification-using-EfficientNet-B0
This repository presents a deep learning–based plant disease classification system built using EfficientNet-B0. The model is trained on a publicly available grape plant disease dataset from Kaggle and is designed to accurately classify multiple plant leaf diseases along with healthy leaves.
The goal of this project is to demonstrate how modern convolutional neural networks (CNNs) can assist in early detection of plant diseases, helping farmers and agricultural experts improve crop health and productivity. 🌱

# Project Overview

Plant diseases significantly affect agricultural productivity and food security. Traditional disease detection methods rely heavily on manual inspection by experts, which can be time-consuming and expensive.

This project uses deep learning and computer vision to automatically detect diseases from plant leaf images.

# The system can:

Identify multiple grape leaf diseases
Distinguish between healthy and infected leaves
Provide fast and accurate classification results
Assist in precision agriculture and smart farming
Dataset

The model is trained using a grape plant disease dataset from Kaggle.

Dataset Features
High-quality images of grape leaves
Multiple disease categories
Includes healthy leaf samples
Suitable for supervised deep learning training
Classes in the Dataset

# The dataset contains several categories such as:

Black Rot
Esca (Black Measles)
Leaf Blight
Healthy Leaves

Each image is labeled according to the disease type or healthy condition.

Model Architecture

This project uses EfficientNet-B0, a lightweight yet powerful convolutional neural network designed for high accuracy with fewer parameters.

Key Features of EfficientNet-B0
Compound scaling method for depth, width, and resolution
Efficient architecture with fewer parameters
Strong performance on image classification tasks
Faster training compared to larger CNN models

EfficientNet-B0 is particularly suitable for plant disease classification because it can extract detailed visual features from leaf images.

Data Preprocessing

Before training, the dataset undergoes several preprocessing steps:

Image resizing
Normalization
Train-validation-test split
Data augmentation
Data Augmentation Techniques

To improve generalization and reduce overfitting, several augmentations are applied:

Random horizontal flip
Random rotation
Random zoom
Brightness and contrast adjustments

These augmentations help the model perform better on real-world leaf images captured in different lighting and environmental conditions.

Training Strategy

The EfficientNet-B0 model is fine-tuned using transfer learning.

Training pipeline:

Load pretrained EfficientNet-B0 weights
Replace the final classification layer
Train on grape leaf disease dataset
Validate model performance
Evaluate accuracy on the test set

Loss function and optimization are configured to ensure stable convergence and improved classification performance.
