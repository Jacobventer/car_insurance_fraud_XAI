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






