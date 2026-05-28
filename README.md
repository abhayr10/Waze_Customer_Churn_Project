# Customer Churn Prediction – Waze Navigation App

## Overview

This project analyzes customer churn behavior in the Waze Navigation App using machine learning and statistical analysis. The objective was to identify patterns associated with user churn and build predictive models capable of detecting at-risk users early.

The project involved exploratory data analysis (EDA), hypothesis testing, feature evaluation, and predictive modeling using Logistic Regression, Random Forest, and XGBoost.

---

## Problem Statement

Waze wanted to better understand why users stop engaging with the platform and identify behavioral signals that indicate potential churn.

The main goal was to:

* Analyze user activity patterns
* Identify statistically significant churn indicators
* Build a classification model to predict churned users
* Prioritize recall to minimize false negatives

---

## Dataset

* Total Records: **14,999**
* Features included:

  * Session activity
  * Drive duration
  * Distance traveled
  * Device type
  * User engagement metrics

---

## Key Insights

* Churned users drove significantly more kilometers despite having shorter sessions, indicating possible over-reliance without long-term engagement.
* Device type showed no statistically significant relationship with user behavior based on a two-sample t-test (p > 0.05).
* Usage-pattern features were more predictive than hardware segmentation features.

---

## Statistical Analysis

### Two-Sample T-Test

Performed hypothesis testing to evaluate whether device type influenced ride behavior.

* Null Hypothesis (H₀): Device type has no effect on user ride behavior
* Result: Failed to reject H₀ (p > 0.05)

This redirected modeling efforts toward behavioral and engagement-based features.

---

## Machine Learning Models

The following models were trained and evaluated:

1. Logistic Regression
2. Random Forest Classifier
3. XGBoost Classifier

### Model Selection Criteria

Models were evaluated using:

* Recall Score
* Precision-Recall Tradeoff
* ROC-AUC Score

The final model prioritized **high recall** to ensure churned users were not missed.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* SciPy

---

## Project Workflow

1. Data Cleaning & Preprocessing
2. Exploratory Data Analysis (EDA)
3. Statistical Hypothesis Testing
4. Feature Engineering
5. Model Training
6. Model Evaluation
7. Business Insights & Recommendations

---

## Results

* Improved churn prediction performance by transitioning from Logistic Regression to ensemble-based models.
* XGBoost delivered the strongest balance between recall and ROC-AUC.
* Generated actionable insights for identifying high-risk users early.

---

## Future Improvements

* Hyperparameter optimization
* Cross-validation improvements
* SHAP interpretability analysis
* Deployment using Flask or Streamlit

---

## Author

Abhay R
Aspiring Data Scientist & Football Video Analyst
