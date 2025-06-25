Credit Risk Analysis using Random Forest
========================================

Overview:
---------
This project uses the "Give Me Some Credit" dataset to build a credit risk classification model using Random Forest. 
The goal is to flag high-risk customers (likely to default) for financial institutions.

Dataset:
--------
• File Used: cs-training.csv
• Source: [Kaggle - Give Me Some Credit](https://www.kaggle.com/c/GiveMeSomeCredit/data)
• Path (update as needed): C:\Users\LENOVO\Downloads\cs-training.csv

Objective:
----------
To build and evaluate a model that:
• Handles missing values using median imputation
• Uses SMOTE to balance the classes
• Applies feature scaling
• Trains a Random Forest model
• Evaluates performance using AUC, classification report, confusion matrix, and ROC curve

Steps:
------
1. **Data Loading & Cleaning**:
   - Missing values handled with median imputation
   - Negative values clipped in 'MonthlyIncome' and 'NumberOfDependents'

2. **Feature Engineering & Scaling**:
   - Data scaled using StandardScaler

3. **Class Imbalance Handling**:
   - SMOTE applied to oversample the minority class

4. **Model Training**:
   - RandomForestClassifier used to train on the balanced dataset

5. **Evaluation Metrics**:
   - Confusion Matrix (heatmap)
   - Classification Report
   - ROC Curve with AUC

Dependencies:
-------------
• Python 3.7+
• pandas
• numpy
• scikit-learn
• matplotlib
• seaborn
• imbalanced-learn
• xgboost (if extended later)

Install dependencies (in your terminal or Anaconda prompt):
-----------------------------------------------------------
pip install pandas numpy scikit-learn matplotlib seaborn imbalanced-learn

Usage:
------
1. Update the dataset path in the script:
   ```python
   data_path = r"C:\Users\LENOVO\Downloads\cs-training.csv"
