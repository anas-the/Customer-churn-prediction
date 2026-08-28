# Customer Churn Prediction

An end-to-end machine learning project built for the **Kaggle Playground Series 2026**, focused on predicting customer churn and translating model outputs into actionable customer-retention insights using ensemble learning techniques.

## 📌 Overview

Customer churn is a critical business metric that directly impacts **revenue, customer lifetime value, and long-term growth**.

This project develops a predictive framework to:

* Identify customers who are at high risk of churning
* Understand the key factors influencing churn
* Compare multiple machine learning models
* Generate actionable insights for customer-retention strategies

**Validation ROC-AUC: 0.917**

---

## 📊 Dataset

* **Source:** Kaggle Playground Series 2026
* **Problem Type:** Binary Classification
* **Evaluation Metric:** ROC-AUC
* **Target Variable:** `Churn`

The dataset contains information related to:

* Customer demographics
* Service subscriptions
* Billing information
* Contract details
* Customer tenure
* Historical usage patterns

---

## 🛠️ Tech Stack

* **Python**
* **Pandas**
* **NumPy**
* **Scikit-learn**
* **XGBoost**

---

## 🔄 Project Workflow

### 1. Data Preprocessing

The dataset was prepared for modeling through the following steps:

* Removed irrelevant identifier columns
* Handled missing values
* Encoded categorical variables
* Standardized feature formats
* Prepared the final feature matrix for model training

### 2. Feature Engineering

Business-oriented features were created to capture customer behavior and value.

#### `AvgSpend`

Average customer spend relative to their tenure, helping capture differences in customer value.

#### `LongTermCustomer`

A tenure-based indicator used to distinguish longer-tenured customers from newer customers.

#### `HighValueCustomer`

A customer segmentation feature designed to identify customers with relatively higher spending/value.

### 3. Model Development

Multiple classification algorithms were implemented and evaluated:

| Model               | Purpose                                        |
| ------------------- | ---------------------------------------------- |
| Logistic Regression | Baseline linear classification model           |
| Random Forest       | Non-linear ensemble baseline                   |
| XGBoost             | Final high-performance gradient boosting model |

The final model was **XGBoost**, selected because it delivered the strongest performance on the structured tabular dataset.

---

## 📈 Results

| Metric                 |     Score |
| ---------------------- | --------: |
| **Validation ROC-AUC** | **0.917** |

The model achieved a **0.917 ROC-AUC** on the validation dataset, demonstrating strong ability to distinguish between customers likely to churn and customers likely to remain.

---

## 🔍 Key Churn Drivers

The analysis identified several variables strongly associated with customer churn:

* **Contract Type**
* **Customer Tenure**
* **Monthly Charges**
* **Internet Service**
* **Online Security**
* **Technical Support**

These factors provide useful signals for identifying customers who may require targeted retention interventions.

---

## 💡 Business Insights

The analysis suggests that customers with the following characteristics have a higher propensity to churn:

* **Month-to-month contracts**
* **Shorter customer tenures**
* **Higher monthly charges**
* **Limited support or security services**

### Potential Retention Strategies

Based on these insights, businesses could consider:

**1. Contract Migration Incentives**
Offer discounts or additional benefits to encourage month-to-month customers to move to longer-term contracts.

**2. Loyalty Programs**
Provide targeted benefits to high-value customers to improve retention and increase customer lifetime value.

**3. Bundled Service Offerings**
Bundle services such as technical support and online security to increase perceived value and reduce churn risk.

**4. Personalized Engagement Campaigns**
Use predicted churn probabilities to prioritize high-risk customers for targeted communication and retention offers.

---

## 📁 Repository Structure

```text
Customer-Churn-Prediction/
│
├── data/
│
├── notebooks/
│   └── churn_prediction.ipynb
│
├── submission.csv
├── requirements.txt
└── README.md
```

---

## 🚀 Future Improvements

Potential extensions to the project include:

* Hyperparameter optimization using **Optuna**
* Model explainability using **SHAP**
* Customer Lifetime Value (CLV) prediction
* Deployment using **Streamlit** or **FastAPI**
* Automated model monitoring and retraining pipelines
* Cost-sensitive churn modeling to prioritize high-value customers

---

## 👤 Author

**Taarini Dagar**

*Business Analytics | Product Management | Machine Learning*

---

## ⭐ Project Highlights

* End-to-end customer churn prediction pipeline
* Business-focused feature engineering
* Comparison of multiple machine learning models
* **0.917 validation ROC-AUC**
* Actionable customer-retention recommendations

