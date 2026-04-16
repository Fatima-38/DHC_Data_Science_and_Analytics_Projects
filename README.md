# 📊 DHC Data Science & Analytics Internship

## Overview

This repository contains all five Data Science & Analytics internship tasks for **DevelopersHub Corporation**. Each task is implemented as a complete Jupyter Notebook featuring data loading, EDA, model training, evaluation, and conclusions.

**Libraries used:** `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`

---

## Tasks

## Task 1 - Exploring and Visualizing a Simple Dataset
**Dataset:** Iris Dataset (via seaborn)  
**Objective:** Read, summarize, and visualize a classic dataset.  
**Approach:**
- Loaded dataset with pandas; inspected shape, columns, dtypes, and `.head()`
- Created scatter plots (sepal & petal dimensions by species), histograms, box plots, pairplot, and a correlation heatmap

**Key Insight:** Petal measurements are far more discriminative than sepal measurements. Petal length and petal width are highly correlated (r = 0.96), making them the strongest features for species classification.

---

## Task 2 - Credit Risk Prediction
**Dataset:** Loan Prediction Dataset (Kaggle structure)  
**Objective:** Predict whether a loan applicant is likely to default.  
**Approach:**
- Handled missing values using mode/median imputation
- Visualized loan amount, income, education, and property area vs loan status
- Trained **Logistic Regression** and **Decision Tree** classifiers
- Evaluated using accuracy score and confusion matrix

**Key Insight:** Credit history is the strongest predictor of loan approval. Applicants without credit history have significantly higher rejection rates.

---

## Task 3 - Customer Churn Prediction (Bank Customers)
**Dataset:** Churn Modelling Dataset  
**Objective:** Identify customers likely to leave the bank.  
**Approach:**
- Cleaned and prepared data; dropped irrelevant columns
- Applied **Label Encoding** (Gender) and **One-Hot Encoding** (Geography)
- Trained **Logistic Regression** and **Random Forest** classifiers
- Analyzed feature importance to understand churn drivers

**Key Insight:** Age, Balance, Number of Products, and inactive membership status are the top churn predictors. Germany has the highest churn rate by geography.

---

## Task 4 - Predicting Insurance Claim Amounts
**Dataset:** Medical Cost Personal Dataset  
**Objective:** Estimate medical insurance charges using regression.  
**Approach:**
- Visualized how BMI, age, and smoking status impact charges
- Trained **Linear Regression** and **Random Forest Regressor**
- Evaluated using **MAE**, **RMSE**, and **R²**

**Key Insight:** Smoking is the dominant cost driver — smokers pay 3–4× more than non-smokers. Random Forest significantly outperforms Linear Regression due to non-linear interactions between features.

---

## Task 5 - Personal Loan Acceptance Prediction
**Dataset:** Bank Marketing Dataset (UCI Machine Learning Repository)  
**Objective:** Predict which customers will accept a personal loan offer.  
**Approach:**
- Explored features: age, job, marital status, education, balance, duration
- Applied Label Encoding and One-Hot Encoding
- Trained **Logistic Regression** and **Decision Tree** classifiers
- Analyzed ROC-AUC and feature importance for business insights

**Key Insight:** Call duration is the strongest predictor. Students and retired customers have the highest subscription rates. Targeting previous successful campaign respondents yields the best conversion rates.

---

> **Note:** All datasets are either loaded via seaborn's built-in loader or simulated programmatically within the notebooks — no external CSV downloads required.

---

## Results Summary

| Task   |            Model Used               |  Metric  | Score |
|--------|-------------------------------------|----------|-------|
| Task 1 | EDA only                            |     —    |   —   |
| Task 2 | Logistic Regression / Decision Tree | Accuracy | ~80%+ |
| Task 3 | Random Forest                       | Accuracy | ~85%+ |
| Task 4 | Random Forest Regressor             |    R²    | ~0.85+|
| Task 5 | Decision Tree                       |   AUC    | ~0.80+|

---
