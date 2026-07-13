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
3. Train/test split
4. Compare Logistic Regression, Decision Tree, and Random Forest Classification & ROC-AUC
5. ROC curve comparison
6. Hyperparameter tuning
7. Feature importance analysis
8. SHAP explainability

## Model Performance
| Metric | Logistic Regression Results | Decision Tree Results | Random Forest Results |
|---------|-----------------------------|-----------------------|-----------------------|
| Accuracy | 0.78 | 0.75 | 0.70 |
| Churn Recall | 0.37 | 0.34 | 0.63 |
| Churn Precision | 0.38 | 0.32 | 0.32 |
| Churn F1 Score | 0.38 | 0.33 | 0.42 |
| ROC-AUC | 0.729 | 0.636 | 0.717 |

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
<img width="580" height="453" alt="download" src="https://github.com/user-attachments/assets/a3804146-a9d7-4a6d-9b85-6ca7f5f552b6" />

<img width="571" height="453" alt="download" src="https://github.com/user-attachments/assets/0a6652f2-aece-4641-91d9-e6e958c55f47" />

<img width="915" height="809" alt="download" src="https://github.com/user-attachments/assets/802ca8b8-70d2-4d7d-bb5b-b5ae937063ed" />

### ROC Curve Comparison
<img width="567" height="453" alt="download" src="https://github.com/user-attachments/assets/fa386a37-7c1f-4337-8666-2b39cb2cb2d6" />

### Feature Importance
<img width="688" height="453" alt="download" src="https://github.com/user-attachments/assets/1e5b4994-6d45-4e3b-8c84-78853a581c48" />

### SHAP Summary Plot
<img width="826" height="466" alt="download" src="https://github.com/user-attachments/assets/53ea9299-9c58-4994-9029-0f0aeacb6dd0" />

## Technologies
- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- SHAP
