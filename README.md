# 📉 Customer Churn Prediction using Logistic Regression

## 📌 Overview

This project uses **Logistic Regression** to predict whether a telecom customer is likely to churn based on demographic information and service-related features.

The project covers data preprocessing, categorical feature encoding, model training, evaluation, and confusion matrix visualization.

---

## 🎯 Objective

The objective is to build a classification model that predicts whether a customer will:

- **Stay** with the company
- **Churn** from the company

---

## 📊 Dataset

**Dataset:** Telco Customer Churn Dataset

The dataset contains information about customer demographics, subscribed services, account details, and churn status.

The dataset contains **7,043 customer records**.

### Target Variable

- `Yes` → Customer churned
- `No` → Customer did not churn

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

---

## ⚙️ Methodology

1. Load the dataset using Pandas.
2. Explore the dataset using `head()`, `info()`, and `describe()`.
3. Identify numerical and categorical features.
4. Convert `TotalCharges` to a numerical data type.
5. Handle missing values in `TotalCharges`.
6. Encode categorical variables.
7. Split the dataset into training and testing sets using an 80:20 stratified split.
8. Train a Logistic Regression classifier.
9. Evaluate the model using Accuracy, Precision, Recall, and F1-Score.
10. Generate a confusion matrix to analyze classification performance.

---

## 🤖 Model

### Logistic Regression

Logistic Regression is used to predict the probability of a customer belonging to the churn class.

The model was trained using the preprocessed customer features.

---

## 📈 Results

The Logistic Regression model achieved the following performance on the test dataset:

| Metric | Score |
|---|---:|
| Accuracy | 79.91% |
| Precision | 64.09% |
| Recall | 55.35% |
| F1-Score | 59.40% |

### Confusion Matrix

```text
                 Predicted
              No       Yes
Actual No     919      116
Actual Yes    167      207