# EcoSort

## Overview
EcoSort is an automated system designed to classify household waste into 10 categories, including garbage, recycling, and organic waste types. The goal is to improve recycling efficiency and enable smart, eco-friendly sorting solutions.

## Dataset
[Garbage Dataset (Kunwar, 2024)](https://www.kaggle.com/datasets/sumn2u/garbage-classification-v2): ~20k images, 10 classes, mix of lab-style and real-world photos.

## Method
We experimented with multiple model architectures:

- ResNet50 trained from scratch
- Vision Transformer (ViT)
- ResNet50 with transfer learning
- ResNet50 with transfer learning, enhanced by CBAM (Convolutional Block Attention Module) and MSFF (Multi-Scale Feature Fusion)

We started with the first two baseline approaches, but noticed modest performance. To improve results, we leveraged pre-trained weights from ImageNet for transfer learning and incorporated enhancements such as Convolutional Block Attention Modules (CBAM) and Multi-Scale Feature Fusion (MSFF). These additions allowed the model to focus on the most informative regions of each image and capture features at multiple resolutions, significantly improving classification accuracy, especially for visually similar waste categories.

## Evaluation
We evaluated model performance using Top-1 and Top-5 accuracy, F1 score, and confusion matrices. These metrics allowed us to assess both overall and per-class performance and identify common misclassification patterns. Full results and visualizations of these metrics can be found in our notebook.
