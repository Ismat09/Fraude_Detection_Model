# Credit Card Fraud Detection
## Introduction

This project builds a machine learning pipeline to detect fraudulent credit card transactions using the "AIML Dataset.csv". It includes exploratory data analysis (EDA), feature engineering, model training, and an exportable prediction pipeline. A Streamlit-based web app is also used to enable interactive fraud prediction.

Fraud detection is a critical component of modern financial systems, helping prevent millions in losses annually

Key features:

Real-time fraud prediction from user inputs
Used **sklearn pipeline** for robust preprocessing & model deployment
Interactive **Streamlit app** lets users simulate transaction scenarios and test fraud risk
Focused on identifying suspicious behavior in **TRANSFER** and **CASH_OUT** transactions

**Results:**
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

