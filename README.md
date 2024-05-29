# Comparison of Support Vector Classifier and Multinomial Naive Bayes for Breast Cancer Diagnosis

## Overview
This project aims to compare the performance of Support Vector Classifier (SVC) and Multinomial Naive Bayes (MNB) algorithms in diagnosing breast cancer using the Wisconsin Breast Cancer dataset. The project involves data preprocessing, exploratory data analysis, feature selection, model training, hyperparameter tuning, and performance evaluation of both classifiers. The goal is to determine which classifier performs better in terms of accuracy and other evaluation metrics.

## Dataset
The dataset used for this project is the Wisconsin Breast Cancer dataset. It consists of 569 instances with 32 attributes, including the diagnosis label ('M' for malignant and 'B' for benign).

## Steps Involved

### 1. Data Loading and Inspection
- Load the Wisconsin Breast Cancer dataset.
- Inspect the dataset for shape, column names, missing values, and data types.

### 2. Data Cleaning
- Drop unnecessary columns such as 'id' and 'Unnamed: 32'.
- Map diagnosis labels ('M' and 'B') to binary values (1 and 0).

### 3. Exploratory Data Analysis (EDA)
- Plot the distribution of each feature using KDE plots.
- Create a bar plot for the diagnosis column.
- Calculate and visualize the correlation matrix using a heatmap.

### 4. Feature Selection
- Identify features highly correlated with the diagnosis variable.

### 5. Model Training and Evaluation
#### Support Vector Classifier (SVC)
- Train and evaluate an SVC model with default parameters on the full feature set.
- Perform grid search for hyperparameter tuning.
- Train and evaluate the SVC model with the best parameters on both the full feature set and the selected correlated features.

#### Multinomial Naive Bayes (MNB)
- Train and evaluate an MNB model with default parameters on the full feature set.
- Perform grid search for hyperparameter tuning.
- Train and evaluate the MNB model with the best parameters on both the full feature set and the selected correlated features.

### 6. Model Performance Comparison
- Combine the performance results of SVC and MNB models into a single bar plot for visualization.
- Compare the accuracy and other evaluation metrics of the models.

## Results
- The Support Vector Classifier (SVC) demonstrated higher accuracy and better performance metrics compared to the Multinomial Naive Bayes (MNB) for diagnosing breast cancer.
- The tuned SVC model with all features achieved the highest accuracy of 98.25%, while the tuned MNB model with selected features achieved an accuracy of 94.74%.

## Conclusion
The Support Vector Classifier (SVC) is a more suitable classifier for the Wisconsin Breast Cancer dataset, especially when using optimal hyperparameters and feature selection techniques.

## How to Run
1. Clone this repository:
2. Navigate to the project directory:
3. Run the Jupyter Notebook to see the full analysis:
