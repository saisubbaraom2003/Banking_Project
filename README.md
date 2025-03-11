# Banking Data Analysis and Prediction

## Overview

This project involves analyzing banking-related datasets, performing data preprocessing, and building machine learning models to predict a target variable. The workflow includes exploratory data analysis (EDA), feature engineering, and model evaluation.

## Data Sources

The following CSV files were used:

- `Geo_scores.csv` - Contains geographical scores.
- `Lambda_wts.csv` - Contains lambda weights.
- `Qset_tats.csv` - Contains Qset TAT scores.
- `instance_scores.csv` - Contains instance scores.
- `test_share.csv` - Contains test data.
- `train.csv` - Contains training data with the target variable.

## Steps Followed

### 1. Data Loading and Exploration

- Read the datasets using `pandas`.
- Checked for missing values, data types, and unique values.
- Merged datasets based on `id` and `Group` columns.

### 2. Data Preprocessing

- Filled missing values using median imputation.
- Encoded categorical variable `Group` using `LabelEncoder`.
- Scaled numerical features using `MinMaxScaler`.
- Split the data into training and testing sets using `train_test_split`.

### 3. Model Training and Evaluation

- Trained multiple classification models:
  - Logistic Regression
  - Decision Tree
  - Random Forest
  - XGBoost
  - K-Nearest Neighbors (KNN)
  - Support Vector Machine (SVM)
  - Naive Bayes
  - Voting Classifier (ensemble model)
- Evaluated models using accuracy scores, cross-validation, and classification reports.
- Visualized the confusion matrix using `seaborn`.

### 4. Predictions on Test Data

- Used the best-performing model (`RandomForestClassifier`) to predict the `Target` variable for the test dataset.

## Results

- The accuracy scores of different models were compared.
- The final predictions were stored in the test dataset.

## Visualizations
- Boxplots for numerical features.
- Confusion matrix heatmap for model evaluation.

 ## Acknowledgments
Data sourced from banking-related datasets.
Libraries used: `pandas`, `numpy` , `matplotlib` , `seaborn` , `scikit-learn`.

---

**Author:** Sai Subba Rao Mahendrakar  
**Date:** 11 March 2025 
