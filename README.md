# House-Prices-Advanced-Regression-Techniques

Machine learning project for predicting house prices using regression models and feature engineering.

---

## 📌 Project Overview

The goal of this project is to predict house prices using a dataset from Kaggle.  
The workflow includes data preprocessing, feature engineering, model selection, and evaluation using cross-validation.

---

## 🧠 Methodology

- Data cleaning and preprocessing
- Log transformation of target variable
- Model comparison using 10-fold cross-validation
- Evaluation metrics: RMSE, MAE, R²
- Final model selection based on composite score

---

## 📊 Models Used

- Linear Regression
- Ridge Regression
- Lasso Regression
- ElasticNet
- Random Forest
- Gradient Boosting

Best model: **ElasticNet**

---

## 📈 Results

- CV RMSE: ~0.11
- Kaggle score: 0.13408
- Stable performance across folds

---

## 🚀 Final Pipeline

- Preprocessing inside sklearn Pipeline
- Cross-validation for model selection
- Final training on full dataset
- Prediction on Kaggle test set

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 📂 Files

- data/: kaggle input datasets
- notebooks/: step-by-step analysis
- submission/: Kaggle output

---

## 📌 Key Insight

Regularized linear models performed best due to the mostly linear structure of the data after transformation.
