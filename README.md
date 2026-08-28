
Customer-Churn-Prediction
An end-to-end machine learning project built for the Kaggle Playground Series 2026, focused on predicting customer churn and deriving actionable retention insights using ensemble learning techniques.

Overview
Customer churn is a critical business metric that directly impacts revenue, customer lifetime value, and growth. This project develops a predictive framework to identify customers at risk of leaving and uncover the key factors influencing churn behavior.

Validation ROC-AUC: 0.917

Dataset
Source: Kaggle Playground Series 2026
Problem Type: Binary Classification
Evaluation Metric: ROC-AUC
Target Variable: Churn
The dataset includes customer demographics, service subscriptions, billing information, contract details, and historical usage patterns.

Tech Stack
Python
Pandas
NumPy
Scikit-learn
XGBoost
Project Workflow
1. Data Preprocessing
Removed identifier columns
Handled missing values
Encoded categorical variables
Standardized feature formats
2. Feature Engineering
Created business-oriented features such as:

AvgSpend: Average customer spend over tenure
LongTermCustomer: Tenure-based retention indicator
HighValueCustomer: Premium customer segmentation
3. Model Development
Implemented and evaluated:

Logistic Regression
Random Forest
XGBoost
The final model utilized XGBoost due to its superior performance on structured tabular data.

Results
Metric	Score
Validation ROC-AUC	0.917
Key Churn Drivers
Contract Type
Customer Tenure
Monthly Charges
Internet Service
Online Security
Technical Support
Business Insights
The analysis revealed that customers with:

Month-to-month contracts
Shorter tenures
Higher monthly charges
Limited support services
show significantly higher churn propensity.

Potential retention strategies include:

Contract migration incentives
Loyalty programs for high-value customers
Bundled service offerings
Personalized engagement campaigns
Repository Structure
├── data/
├── notebooks/
│   └── churn_prediction.ipynb
├── submission.csv
├── requirements.txt
└── README.md
Future Improvements
Hyperparameter optimization using Optuna
SHAP explainability analysis
Customer lifetime value prediction
Deployment using Streamlit or FastAPI
Automated model monitoring pipelines
Author
Mohd Anas and Taarini Dagar

Business Analytics | Product Management | Machine Learning
