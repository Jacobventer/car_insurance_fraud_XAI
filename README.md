# Explainable AI for Car Insurance Fraud Detection

This repository contains the implementation, experiments, and explainability analysis conducted for the bachelor’s thesis:  

Explainable AI for Fraud Detection in Car Insurance: Improving Transparency and Compliance in Machine Learning Models

This project focuses on improving transparency, interpretability and accountability in machine learning bassed fraud detection systems. 
This is to comply to regulations requirements like the General Data Protection Regulation (GDPR).  

## Project Overview

Insurance fraud is a major global challenge, leading to significant financial losses and reduced trust between insurers and clients.
Traditional rule-based systems struggle to detect increasingly complex fraud patterns.

This project explores how machine learning models combined with explainability techniques can improve fraud detection systems.
Fraud detection systems needs Explainability to comply to regulations like GDPR.

The study focuses on:
- Detecting fraudulent car insurance claims
- Comparing interpretable and complex models
- Applying XAI techniques to explain predictions
- Evaluating trade-offs between performance and interpretability


## Research Questions

1.	How do machine learning models (Logistic Regression and Random Forest) perform in detecting fraud in car insurance datasets? 
2.	How can explainable AI techniques (SHAP and LIME) improve the interpretability of fraud detection models? 
3.	To what extent do explainability methods support transparency, accountability, and compliance with regulatory requirements (GDPR) in automated decision-making? 
4.	What are the trade-offs between model performance and interpretability in the context of fraud detection?


## Models Used

- Logistic Regression
- Random Forest baseline
- Random Forest + SMOTE


## Explainability Techniques
- SHAP (Shapley Additive Explanations) - global and local interpretability
- LIME (Local Interpretable Model-agnostic Explanations) – instance-level explanations


## Methodology

- Dataset: Car insurance claims dataset (15,420 records, ~6% fraud rate)
- Data preprocessing:
  - Label encoding
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
│ ├── 03_primary_model_logistic_regression.ipynb  
│ ├── 04_model_random_forest.ipynb  
│ ├── 05_model_comparison.ipynb  
│ ├── 06_shap_analysis.ipynb  
│ ├── 07_lime_analysis.ipynb  
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

- Logistic Regression achieved the highest recall, making it the most effective model in this study for identifying fraudulent claims.
- Random Forest achieved higher precision and ROC-AUC but lower recall.
- Prioritising recall is critical in fraud detection to minimise financial losses.
- SHAP and LIME provided consistent and meaningful explanations:
  - Identified key fraud indicators
  - Enabled transparency in predictions
- Combining interpretable models with XAI may support transparency and accountability requirements associated with GDPR.


## Trade-offs

| Aspect | Logistic Regression | Random Forest |
|------|--------------------|--------------|
| Interpretability | High | Low |
| Recall | High | Lower |
| Precision | Moderate | Higher |
| Transparency | Strong | Requires XAI |


## Limitations

- Use of a public dataset limits real-world generalisation
- Fraud patterns in practice are more complex and dynamic
- SHAP and LIME rely on approximations and may introduce uncertainty


## Future Work

- More advanced XAI trechniques
- Use real-world insurance datasets
- Investigate how analyst use XAI
- Evaluate models in real-time environments


## Installation

```bash
git clone https://github.com/Jacobventer/car_insurance_fraud_XAI.git
cd car_insurance_fraud_XAI
pip install -r requirements.txt
```

## Thesis

This repository supports a bachelor's thesis on:
Explainable AI for Fraud Detection in Car Insurance: Improving Transparency and Compliance in Machine Learning Models


## Author
Jaco Venter

BSc Data Science International University of Applied Science (Germany)  
[LinkedIn Profile](https://www.linkedin.com/in/jaco-venter-45502a162/)

## License

This project is licensed under the MIT License.






