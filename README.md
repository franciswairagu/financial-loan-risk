# Financial Loan Risk Prediction

An end-to-end machine learning project that predicts loan approval decisions using applicants' financial, demographic, and credit-related information. The project follows the **CRISP-DM** methodology and demonstrates the complete data science workflow, from business understanding and exploratory data analysis to model development and evaluation.

---

## Project Overview

Financial institutions must balance approving qualified applicants with minimizing the risk of loan defaults. Manual loan assessment can be time-consuming and inconsistent, making it a suitable candidate for machine learning.

This project develops a binary classification model to predict whether a loan application should be approved. Multiple machine learning algorithms were evaluated, with **Logistic Regression** selected as the final model based on its balanced performance across evaluation metrics.

---

## Business Problem

Loan approval decisions involve balancing two competing objectives:

- Approving creditworthy applicants to maximize business growth.
- Reducing the risk of approving applicants who are likely to default.

The objective of this project is to build a predictive model that supports faster, more consistent, and data-driven lending decisions.

---

## Dataset

- **Source:** Kaggle - Financial Risk for Loan Approval
- **Records:** 20,000 loan applications
- **Features:** 35 variables
- **Target Variable:** `LoanApproved`

The dataset contains applicant demographic, financial, employment, and credit-related information.

---

## Project Workflow

The project follows the CRISP-DM framework:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Exploratory Data Analysis (EDA)
5. Feature Engineering
6. Model Development
7. Model Evaluation
8. Business Recommendations

---

## Exploratory Data Analysis

The EDA focused on:

- Data quality assessment
- Missing value analysis
- Distribution of numerical and categorical features
- Relationship between applicant characteristics and loan approval
- Correlation analysis
- Feature importance

Key findings showed that debt burden, income, and financial stability are among the strongest indicators of loan approval.

---

## Models Evaluated

The following classification algorithms were benchmarked:

- Logistic Regression
- Random Forest
- Gradient Boosting
- Support Vector Machine (SVM)
- XGBoost

---

## Model Performance

| Model | Accuracy | Precision | Recall | F1 Score |
|--------|---------:|----------:|-------:|---------:|
| Logistic Regression | **93%** | **88%** | **85%** | **86%** |
| XGBoost | 90% | **94%** | 63% | 75% |
| Gradient Boosting | 89% | 91% | 60% | 72% |
| SVM | 91% | 85% | 78% | 81% |
| Random Forest | 92% | 80% | 86% | 83% |

### Selected Model

**Logistic Regression**

Although XGBoost achieved the highest precision, Logistic Regression provided the best overall balance between accuracy, precision, recall, and F1-score, making it the preferred model for this project.

---

## Key Features Influencing Loan Approval

Feature importance analysis identified the following variables as the strongest predictors:

- Total Debt-to-Income Ratio
- Monthly Income
- Loan Duration
- Net Worth
- Annual Income
- Total Assets
- Loan Amount
- Bankruptcy History
- Length of Credit History

These findings are consistent with factors commonly considered during credit risk assessment.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- XGBoost
- Jupyter Notebook

---

## Repository Structure

```
Financial-Loan-Risk/
│
├── data/
│   └── Loan.csv
│
├── notebook/
│   └── Financial_Loan_Risk.ipynb
│
├── images/
│
├── README.md
│
└── requirements.txt
```

---

## Results

The final model demonstrates that machine learning can effectively support loan approval decisions by identifying applicants with strong repayment potential while reducing lending risk.

Beyond predictive performance, the project emphasizes:

- Data quality assessment
- Robust preprocessing pipelines
- Model comparison
- Business-oriented evaluation
- Model interpretability

---

## Future Improvements

Potential extensions include:

- Hyperparameter tuning using GridSearchCV
- Threshold optimization for different business objectives
- Class imbalance techniques (SMOTE or class weighting)
- Model deployment using Flask or FastAPI
- Interactive dashboard using Streamlit
- Continuous model monitoring and retraining

---

## Author

**Francis Wairagu**

If you found this project interesting or have feedback, feel free to connect or reach out.