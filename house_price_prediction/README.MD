# House Prices Prediction

This project is based on the Kaggle competition:

House Prices: Advanced Regression Techniques

The main goal was to predict house sale prices using machine learning regression models.

---

# What I Did

In this project, I worked on:

* Data cleaning
* Missing value handling
* Categorical feature encoding
* Log transformation
* Cross-validation
* Ridge Regression
* Hyperparameter tuning
* Kaggle submission generation

---

# Dataset

The dataset contains different house-related features such as:

* Neighborhood
* Garage information
* Basement quality
* Lot area
* Exterior condition
* Sale condition
* Overall quality

Target variable:

* SalePrice

---

# Libraries Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

# Preprocessing

## Missing Values

Different strategies were used depending on the feature:

* Filled some categorical missing values with "None"
* Used median imputation for skewed numerical columns
* Used neighborhood-based median for LotFrontage

---

## Encoding

### Ordinal Encoding

Applied to ordered categorical features such as:

* ExterQual
* BsmtQual
* GarageFinish
* HeatingQC
* KitchenQual

### One-Hot Encoding

Applied to nominal categorical features using `pd.get_dummies()`.

---

## Log Transformation

SalePrice was heavily right-skewed, so I applied log transformation before training the models.

```python
np.log1p(SalePrice)
```

---

# Models Used

## Linear Regression

Used as a baseline model.

## Ridge Regression

Ridge Regression performed much better than Linear Regression after regularization.

I used GridSearchCV to find the best alpha value.

Best parameter:

```python
alpha = 10
```

---

# Evaluation

Used:

* 5-Fold Cross Validation
* RMSE metric

---

# Kaggle Score

Best Public Leaderboard Score:

```text
0.135
```

---

# What I Learned

This project helped me understand:

* Feature preprocessing
* Regularization
* Multicollinearity
* Cross-validation
* Hyperparameter tuning
* End-to-end ML workflow

---

# Future Improvements

Possible future improvements:

* Lasso Regression
* Elastic Net
* XGBoost
* LightGBM
* Feature engineering
* Ensemble models

---

# Author

Rifat
