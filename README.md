# MBATransNet-Skin-Lesion-Segmentation
Deep Learning based Skin Lesion Segmentation using CNN-Transformer Hybrid Network

## Overview

This project presents **MBATransNet**, a hybrid deep learning model for automatic skin lesion segmentation using the **ISIC 2018** dataset. The model combines the local feature extraction capability of Convolutional Neural Networks (CNNs) with the global contextual understanding of Transformers to achieve accurate lesion segmentation.

The architecture also incorporates a Boundary-Aware Attention module and a Dual Decoder to improve segmentation performance, particularly around lesion boundaries.

## Features

- Hybrid CNN-Transformer architecture
- Multi-scale CNN Encoder
- Boundary-Aware Attention (BAA) Module
- Transformer Encoder
- Dual Decoder (Segmentation + Boundary)
- Dice Loss based optimization
- Mixed Precision Training
- Data Augmentation
- Performance evaluation using multiple segmentation metrics

## Dataset

**Dataset:** ISIC 2018 Skin Lesion Analysis Challenge

The dataset contains dermoscopic images and corresponding segmentation masks.

> Note: The dataset is not included in this repository due to its size. It can be downloaded from the official ISIC Challenge website or Kaggle.

## Model Architecture

The proposed MBATransNet consists of:

- Multi-scale CNN Encoder
- Boundary-Aware Attention Module
- Transformer Encoder
- Segmentation Decoder
- Boundary Decoder
- Feature Fusion Module

## Technologies Used

- Python
- PyTorch
- OpenCV
- NumPy
- Albumentations
- Scikit-learn
- Matplotlib
- PIL
- Kaggle Notebook (NVIDIA Tesla T4 ×2 GPU)

## Data Augmentation

The following augmentations were used during training:

- Horizontal Flip
- Vertical Flip
- Random Rotation (90°)
- Gaussian Blur
- CLAHE Contrast Enhancement

## Evaluation Metrics

The model was evaluated using:

- Dice Coefficient
- Intersection over Union (IoU)
- Accuracy
- Precision
- Recall
- F1 Score

## Repository Structure

```
MBATransNet-Skin-Lesion-Segmentation/
│
├── MBATransNet.ipynb
├── README.md
├── requirements.txt
├── .gitignore
│
└── outputs/
    ├── loss_curve.png
    ├── dice_curve.png
    ├── prediction1.png
    └── prediction2.png
```

## Results

The proposed MBATransNet successfully segments skin lesions by combining CNN-based local feature extraction with Transformer-based global feature learning.

Sample prediction results and training curves are available in the **outputs/** folder.

## Future Work

- Extend the model to multi-class lesion segmentation
- Deploy as a web application
- Optimize for real-time inference
- Improve generalization using larger datasets

## Author
**Sayani Konar**
