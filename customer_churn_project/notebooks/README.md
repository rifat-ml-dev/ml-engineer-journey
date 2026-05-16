# Customer Churn Prediction

## Project Overview

This project predicts customer churn using machine learning and business-driven evaluation metrics.

The objective was not only to maximize accuracy, but also to minimize false negatives and identify customers likely to churn.

---

## Dataset

Telco Customer Churn Dataset

* Total samples: 7032
* Features: 30 (after encoding)
* Target:

  * 0 = No churn
  * 1 = Churn

Class distribution:

* No churn: 73%
* Churn: 27%

---

## Project Workflow

### 1. Exploratory Data Analysis

Key findings:

* Month-to-month customers churned significantly more
* Fiber optic customers showed higher churn
* Electronic check users had high churn rates
* Longer tenure reduced churn

### 2. Data Preprocessing

* Removed customer ID
* Handled missing values
* Encoded categorical variables
* Applied feature scaling
* Performed stratified train-test split

### 3. Model Training

Models tested:

* Logistic Regression
* Decision Tree
* Random Forest

### 4. Class Imbalance Handling

Used class-balanced Logistic Regression:

`class_weight='balanced'`

---

## Final Model Performance

Best model:

Logistic Regression (Balanced)

* Accuracy: 73%
* Precision: 49%
* Recall: 79%
* F1 Score: 61%

Confusion Matrix:

```text
[[724 309]
 [ 77 297]]
```

The model successfully identified 297 out of 374 churn customers.

---

## Important Features

Features decreasing churn:

* Two-year contract
* Longer tenure
* Online security
* Tech support

Features increasing churn:

* Fiber optic internet
* Electronic check payment
* Paperless billing
* Streaming services

---

## Tools Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook

---

## Key Learning Outcomes

* Exploratory data analysis
* Feature engineering
* One-hot encoding
* Feature scaling
* Model evaluation
* Overfitting detection
* Bias-variance tradeoff
* Class imbalance handling
* Model interpretability
