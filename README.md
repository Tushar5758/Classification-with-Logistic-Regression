# Breast Cancer Classification using Logistic Regression

## Overview
This project builds a binary classifier to detect breast cancer diagnosis (Malignant or Benign) using logistic regression.

## Dataset
- Dataset loaded from a local CSV file.
- Key columns:  
  - `diagnosis` (target: 'M' = malignant, 'B' = benign)  
  - Multiple numeric features related to tumor characteristics.
- Dataset cleaning includes dropping the `id` column and handling missing values.

## Steps
1. Load dataset and preprocess:
   - Drop `id` column
   - Encode diagnosis labels as 0 (Malignant) and 1 (Benign)
   - Handle missing values with mean imputation
2. Split dataset into train and test (80-20 split, stratified)
3. Standardize features using `StandardScaler`
4. Train Logistic Regression model on training data
5. Evaluate model using:
   - Confusion matrix (heatmap)
   - Classification report (precision, recall, f1-score)
   - ROC curve and ROC-AUC score
6. Experiment with decision threshold tuning and observe changes in confusion matrix
7. Visualize sigmoid function to understand logistic regression probability mapping

## Requirements
- Python 3.x
- scikit-learn
- pandas
- numpy
- matplotlib
- seaborn

## Author
Tushar Deshmukh
