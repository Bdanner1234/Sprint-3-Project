# Project Overview

Customer churn is one of the most pressing challenges for telecom providers. This project predicts whether a customer is likely to leave the company based on their contract details, internet services, and account information.
By identifying customers at risk of churn, the company can take proactive retention measures (e.g., discounts, loyalty programs) to reduce revenue loss.
This project was completed as part of the TripleTen Data Science Program.

Data

The dataset contained the following information about each customer:
Contract details: start and end dates, type of contract, payment method
Internet services: type of connection, additional services (backup, security, etc.)
Account info: monthly charges, total charges, tenure
Target variable: Churn (Yes/No)

Methodology

Data Preprocessing
Replaced EndDate = "No" with active contract values
Encoded categorical features with one-hot encoding
Standardized numerical features
Addressed class imbalance using SMOTE (Synthetic Minority Oversampling Technique)

Model Training

Evaluated multiple models:
Logistic Regression
Random Forest Classifier
Gradient Boosting
Tuned hyperparameters with GridSearchCV

Evaluation Metrics

Main metric: F1-score (threshold ≥ 0.59)
Secondary metric: ROC-AUC for probability-based evaluation

Results

Best model: Random Forest Classifier (after tuning)
F1-score: ~0.60 (met program requirements)
ROC-AUC: ~0.85

Successfully identified customers most at risk of churn

Business Impact: The model provides a tool for targeting retention campaigns, helping reduce customer turnover and increase lifetime value.

Tech Stack

Python
pandas, NumPy, scikit-learn
Matplotlib, Seaborn
imbalanced-learn (SMOTE)
