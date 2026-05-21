# Credit Card Fraud Detection

## Project Overview

This project focuses on detecting fraudulent credit card transactions using machine learning techniques on a highly imbalanced dataset.

The workflow includes:

* Exploratory Data Analysis (EDA)
* Tree-based machine learning models
* Imbalanced data handling techniques
* Precision-Recall analysis
* Threshold tuning
* Cross-validation
* Ensemble learning with Random Forest and XGBoost

The main objective of the project was not only to improve fraud detection performance, but also to understand the tradeoffs between recall, precision, false positives, and false negatives.

---

# Dataset

Dataset: Credit Card Fraud Detection Dataset

### Characteristics

* Highly imbalanced classification problem
* Fraud transactions represent a very small portion of the dataset
* Most features were transformed using PCA for confidentiality

---

# Project Workflow

## 1. Data Understanding and EDA

* Checked dataset structure and missing values
* Analyzed class imbalance
* Visualized fraud distribution
* Explored feature correlations

---

## 2. Baseline Modeling

Started with:

* Logistic Regression
* Decision Tree

This helped establish baseline performance and understand model behavior.

---

## 3. Tree-Based Ensemble Models

Implemented:

* Random Forest
* XGBoost

Learned:

* Bagging vs Boosting
* Overfitting behavior
* Feature importance
* Ensemble learning concepts

---

# Imbalanced Data Handling

Different imbalance handling techniques were explored and compared:

* Oversampling
* Undersampling
* SMOTE
* Class Weight Balancing
* `scale_pos_weight` in XGBoost

The project focused heavily on:

* Recall optimization
* False negative reduction
* Precision-recall tradeoff analysis

---

# Model Evaluation

Models were evaluated using:

* Precision
* Recall
* F1 Score
* ROC-AUC
* Confusion Matrix
* Precision-Recall Curve
* Cross Validation

Threshold tuning was also performed to analyze how changing classification thresholds affected fraud detection performance.

---

# Final Result

Among all models, the strongest overall performance was achieved using:

* Weighted XGBoost
* SMOTE-based Random Forest

These models produced the best balance between:

* Fraud detection capability
* False alarm control

---

# Key Learnings

Through this project, I learned:

* Tree model intuition
* Ensemble learning
* Bagging vs Boosting
* Imbalanced data handling
* Precision vs Recall tradeoff
* Threshold tuning
* Cross-validation
* Practical model evaluation
* Real-world fraud detection challenges

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn
* XGBoost

---

# Project Structure

```text
credit_card_fraud_detection/
│
├── data/
│   └── creditcard.csv
│
├── notebooks/
│   └── fraud_detection.ipynb
│
├── outputs/
│   └── model_comparison_results.csv
│
├── requirements.txt
│
└── README.md
```

---

# Future Improvements

Possible future improvements:

* Hyperparameter tuning
* SHAP explainability
* Model deployment with FastAPI/Flask
* Real-time fraud detection pipeline

---

# Conclusion

This project helped build a strong understanding of classification problems involving highly imbalanced data.

Beyond model training, the project emphasized practical evaluation, business tradeoffs, and model behavior analysis, which are critical in real-world machine learning systems.
