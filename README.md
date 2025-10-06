--Project Overview

This project focuses on predicting customer churn for a telecommunications company. By identifying customers who are likely to leave, the company can proactively take steps to retain them — such as offering discounts or personalized services — and reduce revenue loss.
This work was completed as part of the TripleTen Data Science Program (Sprint 3).

--Data Description

The dataset included customer information such as:
Contract details: start and end dates, payment type, and contract type
Internet services: connection type, additional services (security, backup, etc.)
Customer account info: monthly and total charges, tenure, and demographics

Target variable: Churn (Yes/No)

--Project Steps

Data Preprocessing
Converted “No” in the EndDate column to indicate active customers
Handled missing values and encoded categorical features
Scaled numerical data for consistent model performance

--Exploratory Data Analysis (EDA)

Examined churn patterns across contract types and internet services
Visualized churn vs. total charges, tenure, and contract duration
Model Building

--Tested multiple classification models:

Logistic Regression
Random Forest Classifier
Gradient Boosting (LightGBM)

Used train/test split and cross-validation for fair evaluation

==Evaluation Metrics

Primary metric: F1-score (target ≥ 0.59)
Additional metric: ROC-AUC

--Results

Best model: Random Forest Classifier (after tuning)
F1-score: ≈ 0.60 (met target)
ROC-AUC: ≈ 0.85

The model successfully identified high-risk churn customers for targeted retention campaigns.
Business Value:
This solution allows the telecom company to focus marketing efforts and reduce churn-related revenue loss.
