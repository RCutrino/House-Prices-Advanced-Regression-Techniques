# House Prices - Advanced Regression Techniques

Machine learning project for predicting house prices using regression models and feature engineering.

---

## 📌 Project Overview

The goal of this project is to predict house prices using the Kaggle House Prices dataset.

The workflow includes:
- data preprocessing
- feature engineering
- model comparison
- cross-validation evaluation
- final Kaggle submission

---

## 🧠 Methodology

- Data cleaning and preprocessing using sklearn Pipelines
- Log transformation of the target variable to reduce skewness
- Model comparison using 10-fold cross-validation
- Evaluation metrics: RMSE, MAE, R²
- Model selection based on combined performance metrics and Kaggle leaderboard score

---

## 📊 Models Evaluated

- Linear Regression
- Ridge Regression
- Lasso Regression
- ElasticNet
- Random Forest Regressor
- Gradient Boosting Regressor

### 🏆 Final Model
**ElasticNet Regression (no external feature selection)**

---

## 📈 Results

| Model | Kaggle Score |
|------|-------------|
| ElasticNet (final) | 0.13408 |
| ElasticNet + Feature Selection | 0.13529 |

Cross-validation indicated stable performance across folds with low variance.

---

## 🚫 Feature Selection Experiment

A SelectFromModel approach using ElasticNet was tested to reduce dimensionality.

However:
- it did not improve generalization performance
- it slightly degraded Kaggle score
- ElasticNet already performs implicit feature selection through L1 regularization

Therefore, it was not included in the final pipeline.

---

## 🚀 Final Pipeline

- sklearn Pipeline with preprocessing + model
- full training on complete dataset
- prediction on Kaggle test set

---

## 🛠️ Tech Stack

- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

---

## 📂 Repository Structure

- `data/` → dataset files
- `notebooks/` → EDA and modeling
- `submission/` → Kaggle outputs
- `experiments/` → alternative approaches tested

---

## 📌 Key Insight

Regularized linear models performed best due to the mostly linear structure of the dataset after transformation.

Feature selection did not improve performance, confirming that ElasticNet already provides effective built-in regularization.
