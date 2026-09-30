
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

##  Methodology

### 1. Data Preparation & Cleaning
The raw dataset is inspected to detect data quality issues before analysis:

- Dataset structure and variable inspection
- Duplicate detection
- Missing-value analysis
- Data-type validation
- Categorical-value standardization
- Outlier detection and treatment
- Final data quality checks

### 2. Exploratory Data Analysis (EDA)
EDA investigates the relationship between customer characteristics and churn, focusing on:

- Demographics (age, gender, geography)
- Financial variables (credit score, balance, estimated salary)
- Banking behavior (number of products, credit card ownership, activity status, tenure)
- Class distribution of the target variable `Exited`

### 3. Data Preprocessing
- Feature selection (removal of identifier columns)
- Separation of features and target
- Encoding of categorical variables
- Train-test split
- Feature scaling (for distance/linear-based models)
- Class imbalance handling with **SMOTE** (applied **only on the training set** to avoid data leakage)

### 4. Modeling
Three supervised classification algorithms are compared:

| Model | Why it is used |
|---|---|
| **Logistic Regression** | Interpretable baseline model |
| **K-Nearest Neighbors (KNN)** | Distance-based, non-parametric approach |
| **Random Forest** | Ensemble model capturing non-linear relationships |

### 5. Hyperparameter Tuning
`GridSearchCV` with cross-validation is used to systematically search for the best hyperparameter configuration for each model.

### 6. Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC

> Since churn is an imbalanced problem, **Recall, F1-Score, and ROC-AUC** are prioritized over accuracy alone.
