# EcoSort

## Overview
EcoSort classifies household waste into 3 categories (garbage, recycling, and organic waste) to improve recycling efficiency and enable smart, eco-friendly sorting.

## Notebook
https://colab.research.google.com/drive/1h63ukdj9inxfju6QaTpXGeVe3Ydbq5a9?usp=sharing#scrollTo=-U4V8nk8nsZu

## Dataset
[Garbage Dataset (Kunwar, 2024)](https://www.kaggle.com/datasets/sumn2u/garbage-classification-v2): ~20k images, 10 classes, mix of lab-style and real-world photos.

## Method
We will experiment with CNNs, Vision Transformers, and simple ensembles to handle look‑alike materials and varied lighting/angles.

## Evaluation
Data split: 70% train, 15% validation, 15% test. Tune on validation; report final accuracy on the test set and sanity-check on new real-world images.
