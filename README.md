# CKD Detection using Machine Learning

## Project Overview

This project aims to enhance the early detection and diagnosis of Chronic Kidney Disease (CKD) by leveraging machine learning techniques on both biomarker data and CT scan images. The project includes two primary components:

1. **Biomarker Model:** Implements Random Forest, XGBoost, and SVM for analyzing a dataset with various physiological and biochemical markers.
2. **Imaging Model:** Utilizes a custom Convolutional Neural Network (CNN) for interpreting CT scan images to identify CKD-related abnormalities such as stones, cysts, and tumors.

## Datasets

### Biomarker Data
- **Source:** UCI Machine Learning Repository
- **Description:** 400 samples with 25 features including demographic, physiological, and biochemical data.
- **Preprocessing:** Missing values imputed, features standardized and encoded. Data is split into 80% training and 20% testing sets.

### CT Scan Images
- **Source:** "CT Kidney Dataset: Normal-Cyst-Tumor and Stone" from Kaggle
- **Description:** Images classified into four categories: Normal, Cyst, Tumor, and Stone.
- **Preprocessing:** Custom watershed segmentation, data augmentation, and split into 70% training, 15% validation, and 15% testing sets.

## Model Training

### Biomarker Model
- **Algorithms:** Random Forest, XGBoost, SVM
- **Performance:** 
  - Random Forest: 100% accuracy
  - XGBoost: 100% accuracy
  - SVM: 100% accuracy
- **Cross-Validation:** Stratified K-Fold, Leave-One-Out, and Stratified Shuffle Split

### Imaging Model
- **Model:** Customized Convolutional Neural Network (CNN)
- **Performance:** 
  - Testing Accuracy: 98.66%
  - Validation Accuracy: 99.41%
- **Training:** RMSProp optimizer, categorical cross-entropy loss, fine-tuned with k-fold cross-validation

