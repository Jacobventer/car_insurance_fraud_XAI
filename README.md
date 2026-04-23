# Explainable AI for Car Insurance Fraud Detection

This repository contains the implementaion and analysis for a bachelo's thesis on applyiing Explainable Artificial Intelligence (XAI) to improve  
transparency, interpretability, and regulatory compliance in car insuracne fraud detection.


## Project Overview

Insurance fraud is a major global issue, leading to significant financial losses and reduced trust between insurers and clients.
Traditional rule-based systems struggle to detect increasingly complex fraud patterns.

This project explores how mahcine learning models combined with explainability techniques can improve fraud detection systems.
Fraud detection systems needs explainablity to comply to regulations like GDPR.

The study focuses on:
- Detecting fraudulent car insurance claims
- Comparing interpretable and comple models
- Applying XAI techniques to explain predictions
- Evaluationg trade-offs between perfromance and interpretability


## Research Questions

1.	How do traditional machine learning models (Logistic Regression and Random Forest) perform in detecting fraud in car insurance datasets? 
2.	How can explainable AI techniques (SHAP and LIME) improve the interpretability of fraud detection models? 
3.	To what extent do explainability methods support transparency, accountability, and compliance with regulatory requirements (GDPR) in automated decision-making? 
4.	What are the trade-offs between model performance and interpretability in the context of fraud detection?


## Models Used

- Logistic Regression
- Random Forest
- Baseline model
- SMOTE-enhanced model


## Explainability Techniques
- SHAP (Shapley Additive Explanations) - global and local interpretability
- LIME (Local Interpretable Model-agnostic Explanations) – instance-level explanations


## Methodology

- Dataset: Car insurance claims dataset (15,420 records, ~6% fraud rate)
- Data preprocessing:
  - Label encoding
  - Feature selection
  - Stratified train-test split
- Imbalance handling:
  - Class weighting
  - SMOTE (Synthetic Minority Over-sampling Technique)
- Evaluation metrics:
  - Precision
  - Recall
  - F1-score
  - ROC-AUC

## Project Structure

xai-insurance-fraud-detection/

├── data/
│ ├── raw/
│ ├── processed/ 
│
├── notebooks/
│ ├── 01_data_understanding_and_eda.ipynb
│ ├── 02_data_preprocessing.ipynb
│ ├── 03_logistic_regression_model.ipynb
│ ├── 04_random_forest_model.ipynb
│ ├── 05_model_comparison.ipynb
│ ├── 06_shap_analysis.ipynb
│ ├── 07_lime_analysis.ipynb
│ └── 08_compliance_analysis.ipynb
│
├── results/
│ ├── figures/ 
│ ├── tables/ 
│
├── models/
│ ├── logistic_model/
│ ├── random_forest_baseline/
│ ├── random_forest_SMOTE/
│
├── README.md
├── requirements.txt


## Key Findings

- Logistic Regression achieved the highest recall, making it the most effective model for detecting fraudulent claims.
- Random Forest achieved higher precision and ROC-AUC but lower recall.
- Prioritising recall is critical in fraud detection to minimise financial losses.
- SHAP and LIME provided consistent and meaningful explanations:
- Identified key fraud indicators
- Enabled transparency in predictions
- Combining interpretable models with XAI supports GDPR compliance and improves trust in automated systems.


## Trade-offs

| Aspect | Logistic Regression | Random Forest |
|------|--------------------|--------------|
| Interpretability | High | Low |
| Recall | High | Lower |
| Precision | Moderate | Higher |
| Transparency | Strong | Requires XAI |



