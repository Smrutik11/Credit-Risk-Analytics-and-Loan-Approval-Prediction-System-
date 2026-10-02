# Credit Risk Analytics & Loan Approval Prediction

An end-to-end credit risk analytics project using Python, SQL, and machine learning to analyze loan default risk and build classification models.

The project covers data generation, SQL-based ETL, feature engineering, preprocessing, model training, model evaluation, and saving trained machine learning pipelines.

---

## Project Overview

The objective of this project is to build a reproducible workflow for analyzing borrower and loan characteristics and predicting the probability of loan default.

The project demonstrates:

- Synthetic loan data generation
- SQL-based ETL using SQLite and CTEs
- Data cleaning and preprocessing
- Credit score and DTI risk bands
- Feature engineering
- Logistic Regression
- Random Forest
- ROC-AUC evaluation
- Precision-Recall analysis
- Confusion matrix
- Feature importance
- Saving trained ML pipelines

---

## Business Problem

A lending business needs to understand borrower risk before making loan decisions.

This project transforms loan-level data into an analysis-ready dataset and uses machine learning to estimate default risk.

The workflow answers questions such as:

- Which borrower characteristics are associated with default risk?
- How does credit score relate to default probability?
- How does debt-to-income ratio relate to risk?
- Which features are most important for prediction?
- How do Logistic Regression and Random Forest perform on the test dataset?

---

## Dataset

The project uses a synthetically generated dataset containing **10,000 loan records**.

Each row represents a loan record.

### Key Features

| Feature | Description |
|---|---|
| `loan_id` | Unique loan identifier |
| `loan_amount` | Loan amount |
| `term_months` | Loan term |
| `interest_rate` | Loan interest rate |
| `annual_income` | Borrower's annual income |
| `emp_length_years` | Employment length |
| `credit_score` | Borrower's credit score |
| `dti` | Debt-to-income ratio |
| `num_open_accounts` | Number of open credit accounts |
| `delinquencies_2yrs` | Delinquencies in previous two years |
| `purpose` | Loan purpose |
| `home_ownership` | Home ownership status |
| `age` | Borrower's age |
| `default` | Target variable |

Missing values are intentionally introduced into selected numerical features to demonstrate preprocessing.

---

## Project Workflow

```text
Synthetic Loan Data
        ↓
Data Cleaning
        ↓
SQL ETL using SQLite + CTEs
        ↓
Feature Engineering
        ↓
Credit & DTI Risk Bands
        ↓
Train/Test Split
        ↓
Preprocessing Pipeline
        ↓
Logistic Regression + Random Forest
        ↓
Model Evaluation
        ↓
Feature Importance
        ↓
Save Models & Results
