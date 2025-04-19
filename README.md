# Credit Card Default Risk Prediction Using Machine Learning

This project applies supervised machine learning techniques to predict credit card default risk based on real-world data from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients). The project includes thorough data preprocessing, handling class imbalance, dimensionality reduction using PCA, and performance evaluation across several models.

---

## 📁 Repository Structure

```
Credit-Card-Default-Prediction-ML/
│
├── Credit_Default_Risk_Prediction.ipynb
├── default of credit card clients.xls
├── Credit_Default_Project_Report.pdf
└── README.md
```

---

## 📊 Dataset

- Source: [UCI - Default of Credit Card Clients](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)
- Observations: 30,000 credit card holders
- Target: `default.payment.next.month` (binary: 1 = default, 0 = not default)
- Features include:
  - Demographics (Age, Sex, Education, Marriage)
  - Credit limits and payment status (6 months)
  - Billing amounts and previous payments

---

## 🔍 Project Workflow

### 1. **Exploratory Data Analysis**
- Categorical and continuous variable inspection
- Target distribution analysis (class imbalance)
- Correlation heatmap and feature relationships

### 2. **Data Preprocessing**
- Handling invalid categorical values (e.g., unknown education/marriage categories)
- One-hot encoding of categorical features
- Feature scaling using StandardScaler and MinMaxScaler
- Dimensionality Reduction using PCA

### 3. **Class Imbalance Handling**
- Oversampling: SMOTE (Synthetic Minority Oversampling Technique)
- Undersampling: Cluster Centroid method

### 4. **Classification Models**
- **Logistic Regression** with L2 regularization
- **Decision Tree and Random Forest**
- **Support Vector Machine (SVM)** with RBF Kernel
- Hyperparameter tuning for each algorithm
- Train-test split using stratified sampling

---

## 📈 Evaluation Metrics

- **Accuracy** and **F1-Score**
- **Confusion Matrix**
- **Precision/Recall**
- **AUC-ROC Curve**

> Best results achieved with **SVM + PCA + SMOTE**, reaching an F1-score of **0.5247**.

---

## 📌 Key Highlights

- Applied PCA to retain 99% variance with 12 principal components
- Performed advanced resampling techniques for imbalance management
- Documented comparative performance across models in the final report

---

## 📎 Project Files

- **Credit_Default_Risk_Prediction.ipynb** – Full Jupyter notebook with code and analysis
- **default of credit card clients.xls** – Dataset
- **Credit_Default_Project_Report.pdf** – PDF report with summary, visualizations, and evaluation tables

---

## 🙋‍♂️ Author

**Shiva Kumar Reddy Koppula**  
Graduate Student – Business Analytics  
The University of Texas at Dallas

---

## 🧠 Acknowledgements

- Dataset from Yeh, I. C., & Lien, C. H. (2009), UCI ML Repository
- Guidance from Professor Jason Parker, BUAN 6340 – Spring 2024

---
