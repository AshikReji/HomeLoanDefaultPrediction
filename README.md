# Home Loan Default Prediction

## Overview

Home loan default prediction is a critical problem in the banking and financial sector. Identifying borrowers who are likely to default enables financial institutions to minimize risk, improve lending decisions, and reduce financial losses.

This project develops a Machine Learning classification model that predicts whether a borrower is likely to default on a home loan based on demographic, financial, and loan-related attributes.

---

## Problem Statement

Banks and lending institutions face significant challenges due to loan defaults. Traditional credit assessment methods may not always accurately identify high-risk applicants.

The objective of this project is to build a predictive model that classifies loan applicants as:

* **Default (High Risk)**
* **Non-Default (Low Risk)**

allowing lenders to make data-driven lending decisions.

---

## Dataset

The dataset contains customer loan application records with features such as:

* Applicant Income
* Co-applicant Income
* Loan Amount
* Loan Term
* Credit History
* Property Area
* Employment Information
* Demographic Attributes
* Existing Financial Obligations

### Target Variable

* **Loan Default Status**

  * 0 → Non-Default
  * 1 → Default

---

## Project Workflow

### 1. Data Understanding

* Examined dataset structure and feature distributions.
* Identified missing values and inconsistencies.
* Analyzed class distribution of loan defaults.

---

### 2. Exploratory Data Analysis (EDA)

Performed detailed analysis to understand borrower behavior and default patterns.

Key analyses included:

* Income distribution analysis
* Loan amount distribution
* Credit history impact on defaults
* Property area analysis
* Correlation analysis
* Default rate visualization

Insights from EDA helped identify important risk factors affecting loan repayment.

---

### 3. Data Preprocessing

The following preprocessing techniques were applied:

* Missing value treatment
* Categorical variable encoding
* Feature scaling
* Outlier handling
* Data type conversion

---

### 4. Feature Engineering

Created meaningful features to improve model performance:

* Income-to-loan ratio
* Total household income
* Loan burden indicators
* Credit risk-related features

Feature engineering improved the model's ability to distinguish between high-risk and low-risk applicants.

---

### 5. Handling Class Imbalance

Loan default datasets are typically imbalanced, with significantly fewer default cases than non-default cases.

To address this issue:

* Applied **SMOTE (Synthetic Minority Oversampling Technique)**
* Balanced the training dataset
* Improved minority class prediction capability

---

### 6. Model Development

Built multiple classification models:

* Logistic Regression
* Decision Tree
* Random Forest
* XGBoost

Each model was trained and evaluated using identical preprocessing pipelines.

---

### 7. Hyperparameter Tuning

Optimized model performance using:

* GridSearchCV
* Cross Validation

This helped improve generalization and reduce overfitting.

---

## Model Evaluation

Evaluation metrics used:

* Accuracy
* Precision
* Recall
* F1 Score

### Model Performance

| Model               | Accuracy | Recall | F1 Score |
| ------------------- | -------- | ------ | -------- |
| Logistic Regression | 61.06%   | 56.31% | 18.93%   |
| Decision Tree       | 88.86%   | 6.97%  | 9.18%    |
| Random Forest       | 90.95%   | 4.33%  | 7.17%    |
| XGBoost             | 91.86%   | 4.27%  | 7.81%    |

### Key Observation

Although XGBoost achieved the highest accuracy, Logistic Regression produced significantly higher recall, making it more effective at identifying potential loan defaulters.

Since missing a default borrower is often more costly than incorrectly flagging a safe borrower, recall becomes an important metric in credit risk assessment.

---

## Technologies Used

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Scikit-learn
* XGBoost
* Imbalanced-learn (SMOTE)

### Visualization

* Matplotlib
* Seaborn

### Model Selection

* GridSearchCV
* Cross Validation

---

## Key Skills Demonstrated

* Data Cleaning
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Class Imbalance Handling
* SMOTE Implementation
* Classification Modeling
* Hyperparameter Tuning
* Model Evaluation
* Credit Risk Analytics

---

## Project Structure

```text
Home-Loan-Default-Prediction/
│
├── data/
├── notebooks/
├── models/
├── reports/
├── requirements.txt
├── README.md
└── home_loan_default_prediction.ipynb
```

---

## Future Improvements

* Implement cost-sensitive learning techniques.
* Experiment with CatBoost and LightGBM.
* Apply advanced feature selection methods.
* Develop an explainable AI dashboard using SHAP.
* Deploy the model using Streamlit or Flask.

---

## Conclusion

This project demonstrates an end-to-end machine learning workflow for credit risk assessment. By leveraging data preprocessing, feature engineering, SMOTE, and multiple classification algorithms, the solution provides valuable insights into borrower default risk and supports informed lending decisions.

---

## Author

**Ashik Reji**
**Data Science | AI Engineer**

GitHub: [https://github.com/AshikReji](https://github.com/AshikReji)

LinkedIn: [https://linkedin.com/in/ashikreji/](https://linkedin.com/in/ashikreji/)
