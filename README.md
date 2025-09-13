# Alzheimer-Detection
📌 Overview
This project implements an AI-based system for early dementia detection using MRI brain scans. It leverages Gabor feature extraction and machine learning classifiers (SVM, Random Forest) to distinguish between demented and non-demented patients with high accuracy.

By combining medical image preprocessing, texture-based feature extraction, and robust ML models, the project demonstrates the potential of AI in healthcare diagnostics, specifically for Alzheimer’s and dementia screening.


🎯 Key Features
MRI brain scan dataset with 6,400 images across different dementia stages
Preprocessing: resizing, noise reduction, train/test split (80:20)

Feature extraction:
GLCM (Gray-Level Co-occurrence Matrix) → baseline accuracy (~70%)
Gabor Filters → boosted accuracy (~93%)

Classification models: Support Vector Machine (SVM), Random Forest
Cross-validation (5-fold) to validate robustness


📂 Dataset
Source: Kaggle – MRI Dementia Brain Images
Classes:
Mild Demented (896 images)
Moderate Demented (64 images)
Very Mild Demented (2240 images)
Non-Demented (3200 images)


📊 Results
| Method                            | Classifier        | Accuracy  |
| --------------------------------- | ----------------- | --------- |
| GLCM                              | SVM               | 62.8%     |
| GLCM                              | Random Forest     | 69.8%     |
| **Gabor Filter**                  | **SVM**           | **93.6%** |
| **Gabor Filter**                  | **Random Forest** | **93.7%** |


