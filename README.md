# Predicting Brain Stroke Using Machine Learning Models

## Overview
This repository contains a machine learning framework designed to predict the likelihood of a brain stroke using demographic, medical, and lifestyle-related data. The objective is to provide automated risk prediction to assist healthcare practitioners with early stroke detection and proactive medical interventions.

## Dataset
The project utilizes a publicly available Kaggle Stroke Prediction dataset consisting of around 5000 patient records. 
* **Features:** The dataset includes 11 attributes such as gender, age, hypertension, heart disease, marital status, work type, residence type, average glucose level, BMI, and smoking status. 
* **Preprocessing:** The data preprocessing pipeline includes feature scaling for numerical characteristics and one-hot encoding for categorical variables. To handle extreme class imbalance in the target variable, a combination of random oversampling and undersampling was applied.

## Machine Learning Models
Five supervised learning models were implemented and evaluated using an 80:20 stratified train-test split:
* **Logistic Regression:** Used as a baseline model for its simplicity and interpretability.
* **Random Forest:** An ensemble method used to capture intricate relationships and nonlinear feature interactions.
* **Gradient Boosting:** Employed to sequentially correct previous errors and enhance predictive performance.
* **Support Vector Machine (SVM):** Used to construct an optimal decision boundary for binary classification.
* **K-Nearest Neighbors (KNN):** Implemented to evaluate the influence of local data patterns on stroke prediction.

## Key Results
* **Best Model:** The Random Forest classifier achieved the highest predictive performance with an accuracy of approximately 97.25% and an F1-score of 0.97.
* **Model Comparisons:** Logistic Regression and Gradient Boosting also showed strong ability to discriminate between stroke and non-stroke patients, achieving the highest AUC scores. 
* **Feature Importance:** Feature analysis indicated that age, average glucose level, hypertension, and BMI were among the most critical factors contributing to stroke prediction.
