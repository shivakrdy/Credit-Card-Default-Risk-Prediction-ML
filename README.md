# Credit Card Default Risk Prediction – Machine Learning Pipeline

[![Python](https://img.shields.io/badge/Python-Data--Science-blue?logo=python)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-Data--Wrangling-yellow?logo=pandas)](https://pandas.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)](https://jupyter.org/)
[![UT Dallas](https://img.shields.io/badge/UTD-Project-green?logo=academia)](https://www.utdallas.edu/)

This repository showcases a data-driven approach to predicting credit card default using real-world behavioral and financial data. The project covers an end-to-end pipeline — from preprocessing and feature engineering to dimensionality reduction and advanced classification — built to simulate a real-world credit risk scoring system.

---

## Objective

To develop a supervised learning model that accurately predicts whether a client will default on their credit card payment in the upcoming month. The goal is to extract actionable insights from behavioral features and optimize model performance in the presence of imbalanced classes.

---

## Dataset

- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- **Records:** 30,000 credit card clients
- **Features:**
  - Demographics: Age, Sex, Education, Marital Status
  - Credit and payment history (last 6 months)
  - Past bill amounts and repayments
- **Target Variable:** `default.payment.next.month`  
  *(1 = default, 0 = not default)*

---

## 🗂️ Repository Contents

```
Credit-Card-Default-Prediction-ML/
│
├── Credit_Default_Risk_Prediction.ipynb       # Full analysis and model pipeline
├── default_of_credit_card_clients.xls         # Dataset
├── Credit_Default_Project_Report.pdf          # Formal PDF report with insights
└── README.md
```

---


## Project Pipeline

### Exploratory Data Analysis (EDA)
- Identified class imbalance and skewness in features
- Correlation matrix and statistical distributions
- Uncovered hidden patterns in repayment behavior and bill history

### Preprocessing
- Handled invalid and unknown categorical values
- Applied one-hot encoding for nominal categories
- Scaled numerical features using MinMaxScaler and StandardScaler

### Dimensionality Reduction
- Applied **PCA** to reduce multicollinearity and capture 99% variance
- Final model trained on top 12 principal components

### Imbalanced Data Strategy
- Addressed class imbalance using:
  - **SMOTE (Synthetic Minority Oversampling Technique)**
  - **Cluster Centroids (undersampling)**
  - Stratified train-test split

### Models Trained
- **Logistic Regression**
- **Decision Tree**
- **Random Forest**
- **Support Vector Machine (SVM)**
- Used GridSearchCV and cross-validation for hyperparameter tuning

---

## Evaluation Metrics

- Accuracy, Precision, Recall, F1-Score
- Confusion Matrix and Classification Report
- ROC Curve and AUC Score
- Comparative Model Performance Summary

> **Best Model:** SVM with PCA + SMOTE  
> Demonstrated strong recall under balanced sensitivity-precision tradeoff

---


## Key Insights

- Clients aged 30–40 had the highest risk of default
- High credit limits didn’t correlate with repayment reliability
- Late payments in recent months are top predictors of default
- Dimensionality reduction with PCA improved model generalizability

---

## Tech Stack

- **Language:** Python 3.8+
- **IDE:** Jupyter Notebook
- **Libraries:** pandas, numpy, seaborn, matplotlib, scikit-learn, imblearn
- **Techniques:** PCA, SMOTE, Class Balancing, SVM, Tree-based models

---

## 👤 Author

**Shiva Kumar Reddy Koppula**  
Graduate Student – Artificial Intelligence & Business Analytics  
The University of Texas at Dallas  
GitHub: [@shivakrdy](https://github.com/shivakrdy)

---

## References

- UCI Credit Default Dataset: Yeh, I. C., & Lien, C. H. (2009)
- Course: Predictive Analytics, Spring 2024, Instructor: Jason Parker

---

