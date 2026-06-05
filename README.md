<h1 align="center">Kaggle Notebooks</h1>
<p align="center"><em>A collection of end-to-end ML notebooks spanning regression, classification, and generative modelling.</em></p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-58A6FF?style=flat-square&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Jupyter-Notebook-7C3AED?style=flat-square&logo=jupyter&logoColor=white" alt="Jupyter">
  <img src="https://img.shields.io/badge/scikit--learn-ML-58A6FF?style=flat-square&logo=scikit-learn&logoColor=white" alt="scikit-learn">
  <img src="https://img.shields.io/badge/TensorFlow-2.x-7C3AED?style=flat-square&logo=tensorflow&logoColor=white" alt="TensorFlow">
  <img src="https://img.shields.io/badge/Kaggle-Profile-58A6FF?style=flat-square&logo=kaggle&logoColor=white" alt="Kaggle">
</p>

---

## Overview

This repository contains Jupyter notebooks written for Kaggle competitions and learning exercises. Each notebook is self-contained with data loading, exploratory data analysis, model training, and evaluation.

> Kaggle profile: [kaggle.com/vaishakgkumar](https://www.kaggle.com/vaishakgkumar)

---

## Notebooks

### Boston House Price Prediction

**File:** `boston-house-prediction.ipynb`

Predicts median house values in Boston suburbs using the classic Boston Housing dataset. Covers EDA with histograms and correlation heatmaps, feature analysis, and a Linear Regression baseline.

**Techniques:** Linear Regression · scikit-learn · pandas · matplotlib

---

### Credit Card Fraud Detection

**File:** `credit-card-fraud-detection.ipynb`

Binary classification on a highly imbalanced dataset (Kaggle Credit Card Fraud dataset). Compares multiple classifiers on both the original imbalanced set and a balanced undersampled version.

**Models compared:** Logistic Regression · Shallow Neural Network (Keras) · Random Forest · Gradient Boosting · Linear SVM

**Techniques:** RobustScaler · train/val split · `classification_report` (precision/recall/F1) · class imbalance handling · undersampling

---

### Generating Fake Faces with GANs

**File:** `generating-fake-faces-using-gan.ipynb`

Implements a Generative Adversarial Network from scratch in TensorFlow/Keras to synthesise photorealistic face images. Explains GAN theory (generator/discriminator adversarial loop, Gaussian latent space) before building both networks with Conv2D, BatchNormalization, and LeakyReLU layers.

**Architecture:** DCGAN-style · latent dim 100 · 128×128 RGB output · custom training loop with `generator_loss` / `discriminator_loss`

**Techniques:** TensorFlow 2 · Keras Sequential API · Conv2D downsampling/upsampling · adversarial training

---

## Project Structure

```
Kaggle-Notebooks/
├── boston-house-prediction.ipynb       # Regression — Boston Housing dataset
├── credit-card-fraud-detection.ipynb   # Classification — imbalanced fraud detection
└── generating-fake-faces-using-gan.ipynb  # Generative — DCGAN face synthesis
```

---

## Running the Notebooks

Each notebook is designed to run on Kaggle or locally with the standard scientific Python stack.

```bash
# Install dependencies (if running locally)
pip install numpy pandas matplotlib scikit-learn tensorflow keras

# Launch Jupyter
jupyter notebook
```

For the fraud detection notebook, download the dataset from [Kaggle](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) and update the path in the first cell.

For the GAN notebook, download the [CelebA](https://www.kaggle.com/datasets/jessicali9530/celeba-dataset) or equivalent face dataset and update the input path accordingly.

---

## License

This project is licensed under the terms of the [MIT License](LICENSE).
