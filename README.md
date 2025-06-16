# Credit Card Fraud Detection
## Introduction

This project builds a machine learning pipeline to detect fraudulent credit card transactions using the "AIML Dataset.csv". It includes exploratory data analysis (EDA), feature engineering, model training, and an exportable prediction pipeline. A Streamlit-based web app is also used to enable interactive fraud prediction.

Fraud detection is a critical component of modern financial systems, helping prevent millions in losses annually

## Key features:

-Real-time fraud prediction from user inputs
-Used **sklearn pipeline** for robust preprocessing & model deployment
-Interactive **Streamlit app** lets users simulate transaction scenarios and test fraud risk
-Focused on identifying suspicious behavior in **TRANSFER** and **CASH_OUT** transactions

## Data Preprocessing
-Reads in AIML Dataset.csv
Data cleaning steps:
-Missing value checks
-Feature engineering: creates balanceDiffOrig and balanceDiffDest
-Drops unneeded columns: "step", "nameOrig", "nameDest", "isFlaggedFraud"
-One-hot encoding for "type" categorical variable
-Standard scaling for numerical features

## 📌 Exploratory Data Analysis (EDA)
## Visualizations of:
- Transaction types distribution
- Fraud rate per transaction type
- Transaction amount distribution (log)
- Fraud over time
- Correlation matrix
- Fraud distribution in "TRANSFER" and "CASH_OUT" types

## Business insights:
- Fraud concentrated in "TRANSFER" and "CASH_OUT"
- Suspicious balance changes detected (zero_after_transfer subset)

## 📌 Model Training & Evaluation
## Model: Logistic Regression with balanced class weights
- Pipeline used:
- ColumnTransformer for preprocessing
- LogisticRegression model
## Model performance:
- Classification report: good recall for fraud detection, precision could improve
- Confusion matrix printed
- Train/test split: 70/30, stratified

Pipeline exported as: fraud_detection_pipeline.pkl 

## Results:
- Achieved good recall on highly imbalanced data
- Interactive app makes the project suitable for demo to recruiters / clients
- Supports risk-based decisioning for financial transactions
-Achieved good recall on highly imbalanced data and interative App.

**Streamlit App - 95% Accuracy**
## How to use:
- Select Transaction Type from dropdown.
- Enter Transaction Amount.
- Enter sender and receiver balances.
- Click Predict.

The app will display whether the transaction is predicted as Fraud (0) or Not Fraud(1).

