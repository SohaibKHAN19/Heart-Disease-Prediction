This is a solid end-to-end ML project—you’ve covered **EDA → preprocessing → modeling → evaluation → explainability → business insight**,
which is exactly what recruiters want. I’ll give you two things:


---


#  Heart Disease Prediction & Risk Analysis

# Project Overview:

This project builds a complete machine learning pipeline to **predict the likelihood of heart disease** and provide **interpretable insights** into the
key risk factors influencing predictions.

The goal is not only to classify patients as *disease / no disease*, but also to:

* Explain *why* a prediction was made
* Identify **primary risk factors per patient**
* Provide **data-driven insights for healthcare decisions**



# Problem Statement

Heart disease is one of the leading causes of death worldwide. Early detection can significantly improve outcomes.

This project aims to:

* Predict heart disease using patient medical data
* Compare multiple ML models
* Provide **explainable AI insights (SHAP + feature contribution)**



# Dataset

The dataset contains patient health attributes such as:

* Age
* Blood Pressure
* Cholesterol
* Heart Rate
* Chest Pain Type
* ECG Results
* Exercise Induced Angina
* Thalassemia
* Target (0 = No Disease, 1 = Disease)



# Data Preprocessing

Steps performed:

* Replaced invalid values (`-`) with `NaN`
* Filled missing values using **median**
* Separated:

  * Numerical features → StandardScaler
  * Categorical features → OneHotEncoder
* Used **ColumnTransformer** for clean pipeline processing



# Exploratory Data Analysis (EDA)

* Correlation heatmap
* Boxplots (numerical vs target)
* Countplots (categorical vs target)
* Class imbalance visualization
* Feature distributions



# Models Used

* Logistic Regression
* Decision Tree
* Naive Bayes

✅ Used **Pipeline** to avoid data leakage
✅ Used **Cross Validation (CV=5)** for reliable performance



# Hyperparameter Tuning

* GridSearchCV used for Logistic Regression
* Tuned parameter:

  * `C` (Regularization strength)



 Model Evaluation Metrics

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC Curve & AUC


# Results Comparison

* Compared all models visually using:

  * Bar charts
  * ROC curves



# Explainability (Key Highlight 🚀)

This project goes beyond prediction:

# 1. SHAP Analysis

* Global feature importance
* Individual prediction explanation (waterfall plots)

# 2. Feature Contribution Analysis

* Calculated:


  Contribution = Feature Value × Model Weight
  
* Identified:

  * **Primary Risk Factor per patient**
  * **% contribution of each feature**



# Decision Tree Interpretation

* Full tree visualization
* Simplified tree (depth=3)
* Feature importance ranking
* Text-based tree rules



# Output Files

Generated reports:

* `heart_disease_results.xlsx`
* `heart_disease_detailed_analysis.csv`
* `heart_disease_full_probability_report.csv`

These include:

* Predictions
* Probabilities
* Risk factors
* Feature contribution percentages



# Key Insights

* Certain features strongly influence predictions (e.g., chest pain, cholesterol, oldpeak)
* Model interpretability helps understand **why patients are at risk**
* Logistic Regression performed best overall



# Tech Stack

* Python
* Pandas, NumPy
* Seaborn, Matplotlib
* Scikit-learn
* SHAP

