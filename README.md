# 📉 Customer Churn Prediction using Logistic Regression

A machine learning project that predicts customer churn using Logistic Regression on the Telco Customer Churn dataset.

## 📌 Overview

This project implements an end-to-end classification workflow to predict whether a customer is likely to churn.

The workflow includes data exploration, missing-value handling, categorical encoding, train-test splitting, Logistic Regression training, and evaluation using classification metrics and a confusion matrix.

## 🎯 Objectives

- Explore the Telco Customer Churn dataset
- Identify numerical and categorical features
- Handle missing values
- Encode categorical variables
- Remove unnecessary identifier columns
- Train a Logistic Regression classifier
- Evaluate churn predictions using multiple classification metrics

## 📊 Dataset

The project uses the **Telco Customer Churn Dataset**.

The dataset contains **7,043 customer records** and 21 original columns.

### Target Variable

`Churn`

| Value | Meaning |
|---|---|
| `Yes` | Customer churned |
| `No` | Customer did not churn |

The `customerID` column was removed before model training.

## ⚙️ Data Preprocessing

### Missing Values

`TotalCharges` was initially stored as an object/string column.

It was converted to numeric values using:

```python
pd.to_numeric(df["TotalCharges"], errors="coerce")
