
#  Bank Customer Churn Prediction

## Project Overview

Customer churn is an important business problem in the banking sector. Understanding which customers are likely to leave can help financial institutions identify patterns in customer behavior and support data-driven retention strategies.

This project applies a machine learning approach to a bank customer dataset in order to explore customer characteristics associated with churn and develop classification models for predicting customer exit.

The project includes data exploration, data cleaning, preprocessing, machine learning model development, and model evaluation.

---

##  Project Objective

The main objective of this project is to analyze bank customer data and build machine learning models capable of predicting whether a customer is likely to leave the bank.

The target variable is:

- `Exited = 0` → Customer did not leave the bank
- `Exited = 1` → Customer left the bank

The project also aims to identify relevant customer characteristics and patterns that can provide useful business insights.

---

##  Dataset

The dataset contains customer demographic, financial, and banking-related information.

The main variables include:

| Variable | Description |
|---|---|
| `CustomerId` | Unique customer identifier |
| `Surname` | Customer surname |
| `CreditScore` | Customer credit score |
| `Geography` | Customer location |
| `Gender` | Customer gender |
| `Age` | Customer age |
| `Tenure` | Number of years with the bank |
| `Balance` | Customer account balance |
| `NumOfProducts` | Number of products used by the customer |
| `HasCrCard` | Whether the customer has a credit card |
| `IsActiveMember` | Whether the customer is an active member |
| `EstimatedSalary` | Estimated customer salary |
| `Exited` | Customer churn indicator / target variable |

---

##  Project Workflow

The project follows the following workflow:

```text
Raw Dataset
     │
     ▼
Data Exploration
     │
     ▼
Data Quality Assessment
     │
     ▼
Data Cleaning
     │
     ▼
Data Preprocessing
     │
     ▼
Exploratory Analysis
     │
     ▼
Machine Learning Models
     │
     ▼
Model Evaluation
     │
     ▼
Business Interpretation
