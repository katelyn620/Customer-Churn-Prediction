# Customer Churn Prediction using Machine Learning

## Overview
This project predicts customer churn for a fictional SaaS company using machine learning.

A synthetic dataset of 7,500 customers was generated using a logistic risk model to simulate realistic customer behavior and churn patterns.

The goal is to identify customers at risk of leaving based on:
- Customer satisfaction
- Tenure
- Product engagement
- Support interactions
- Subscription characteristics

## Business Problem
Customer churn directly impacts revenue and growth. 

This project aims to identify at-risk customers early enough for retention teams to intervene with personalized offers and support.

## Dataset Features

| Feature | Description | Measurement |
|----------|-------------|-----------|
| age | Customer age | Years |
| tenure_months | How long a customer has been subscribed | Months |
| monthly_cost | Monthly subscription fee | USD |
| support_tickets | Customer support interactions | Integer |
| login_frequency | Monthly logins | Integer |
| feature_usage_score | Product engagement score | Integer from 1-100 |
| satisfaction_score | Customer satisfaction rating | Integer from 1-10 |
| monthly_contract | Monthly vs. annual billing | 0 for annual, 1 for monthly |
| premium member | Premium subscription status | 0 for non-premium, 1 for premium |
| churn | Whether a customer stays subscribed (target variable) | 0 for stay, 1 for churn |
| churn_label | Label for if customer stays or churns | Stayed or Churned |

## Machine Learning Pipeline
1. Synthetic data generation
2. Exploratory Data Analysis (EDA)
3. Feature engineering
4. Train/test split
5. Compare Logistic Regression, Decision Tree, and Random Forest Classification
6. Hyperparameter tuning
7. ROC-AUC evaluation
8. Feature importance analysis
9. SHAP explainability

## Model Performance
Logistic Regression Results
- Accuracy:
- Churn Recall:
- Churn Precision:
- Churn F1 Score:
- ROC-AUC:

- Decision Tree Results
- Accuracy:
- Churn Recall:
- Churn Precision:
- Churn F1 Score:
- ROC-AUC:

- Random Forest Results
- Accuracy:
- Churn Recall:
- Churn Precision:
- Churn F1 Score:
- ROC-AUC:

## Key Findings
Random Forest model was the best performing.

SHAP analysis identified the strongest churn predictors:
1. Satisfaction Score
2. Tenure
3. Monthly Contract Status
4. Premium Membership
5. Support Ticket Volume

Customers with lower satisfaction and shorter tenure exhibited the highest churn risk.

## Visualizations

### Feature Importance

### SHAP Summary Plot

## Technologies
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- SHAP
