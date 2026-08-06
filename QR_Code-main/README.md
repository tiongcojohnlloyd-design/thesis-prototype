# QR Code Authentication App

This project implements a machine learning-based system to distinguish between **original** and **counterfeit** QR code prints using image texture analysis.

## 🔍 Objective

The aim is to classify scanned or photographed QR code images into two categories:
- **Original** (label: 0)
- **Counterfeit** (label: 1)

## 📁 Dataset Structure

Images are read from two folders:
- `Original` QR codes
- `Counterfeit` QR codes

> Note: Modify folder paths in the notebook to match your local structure.

## ⚙️ Features Used

Images are processed in grayscale and passed through multiple feature extraction methods:
- **Global Histogram** of pixel intensities
- **Edge Histogram** using Canny edge detection
- **Local Binary Pattern (LBP)**
- **Gray-Level Co-occurrence Matrix (GLCM)** features like contrast, dissimilarity, homogeneity, energy, correlation, and ASM

## 🧠 Machine Learning Models

The following classifiers are trained and tested:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Machine (SVM)
- Random Forest
- Gradient Boosting Classifier

## 📊 Evaluation Metrics

Each model is evaluated using:
- **Accuracy Score**
- **Classification Report** (Precision, Recall, F1-Score)

## 🖼️ Visualization

The notebook also includes visualizations:
- Sample images with labels
- Bar plots to compare classifier accuracies

## 🛠️ Requirements

Install dependencies using pip:

```bash
pip install opencv-python scikit-image matplotlib scikit-learn numpy

