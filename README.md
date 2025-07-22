# Bank_Customer_Churn_Predictor

## Project Overview
This project predicts customer churn for credit card holders in a banking dataset, aiding finance industry retention strategies. It includes comprehensive EDA with categorical and numerical features, data cleaning via encoding, custom feature engineering (e.g., transaction amount per count), and Scikit-Learn models with feature selection based on importance.

## Key highlights:

# Dataset: 
Bank Churners from Kaggle (10,127 samples, 21 features including demographics, transaction behavior, etc.).

# Techniques:
EDA with count plots for categoricals, histograms, correlation heatmaps, boxplots by churn; one-hot encoding and handling of 'Unknown' categories.
Models: Logistic Regression, Random Forest, SVM with class weights for imbalance.
# Metrics:
F1 Score, ROC AUC.
# Originality:
Custom interaction feature (Total_Trans_Amt_per_Ct); feature selection using Random Forest importances for model refinement.
This project highlights skills in customer analytics, feature engineering, and predictive modeling for financial services.

# Requirements
Python 3.x
Jupyter Notebook
Libraries:
numpy
pandas
matplotlib
seaborn
scikit-learn
Install via:



## Dataset
Download the dataset from Kaggle: Credit Card Customers. Place BankChurners.csv in the project directory.

## How to Run
Open the Jupyter Notebook bank_churn_prediction.ipynb in Jupyter Lab or Notebook.
Ensure the dataset file is in the same directory.
Run all cells sequentially. The notebook drops unnecessary columns and handles encoding automatically.
Outputs include churn distribution plots, model results table, and feature importance bar chart.
File Structure
bank_churn_prediction.ipynb: Main Jupyter Notebook with all code and explanations.
BankChurners.csv: Dataset file (download separately).
README.md: This file.
## Results Example
Churn rate ~16%; balanced models perform well:

Logistic Regression: F1 ~0.75, ROC AUC ~0.92
Random Forest: F1 ~0.85
SVM: F1 ~0.80
Top features like Total_Trans_Ct drive predictions.

Limitations and Future Work
Handle 'Unknown' categories more robustly (e.g., imputation).
Add time-series analysis if longitudinal data available.
Build a dashboard with Dash for interactive churn risk assessment.
