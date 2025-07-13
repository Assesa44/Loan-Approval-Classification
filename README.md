# Loan Approval Classifier

A machine learning project to predict whether a loan application will be approved or not, using data from a real-world financial institution.

---

## Project Overview

This project was built to simulate an intelligent loan decision system used by digital lenders or financial institutions. Using customer information like marital status, employment, credit history, and more, the model learns to classify whether a loan should be **approved (1)** or **rejected (0)**.

---

## Problem Statement

Manual loan approvals are slow, subjective, and prone to bias.  
The goal of this project is to build a **classification model** that can automate this decision reliably and fairly.

---

## Dataset

The dataset was sourced from a public domain Kaggle repository.  
It contains 600+ records with the following features:

- Gender
- Marital Status
- Dependents
- Education
- Self Employment
- Applicant & Coapplicant Income
- Loan Amount & Term
- Credit History
- Property Area
- Loan Status (Target Variable)

> Missing values were cleaned and categorical variables were encoded.

---

## Model Development

We tested multiple classification models:
- Logistic Regression (with class balancing)
- Random Forest ✅ (best performer)
- Support Vector Machine (underperformed)

> After comparing F1-scores and confusion matrices, **Random Forest** emerged as the most accurate and fair model.

---

## Results

- **Accuracy**: 78%
- **F1 Score (Class 1 - Approved)**: 0.85
- **Recall (Class 1)**: 96%
- **Precision (Class 0 - Rejected)**: 0.86

The model is slightly biased toward approvals, which can be fine-tuned further through hyperparameter optimization or better balancing techniques.

---

## Tech Stack

- Python
- Pandas, NumPy
- scikit-learn
- Joblib (for model serialization)

---

## 📁 Project Structure

Loan_Approval_Classifier/
├── Data/
├── Models/
├── Notebooks/
├── main.py (optional)
├── requirements.txt
└── README.md

---

## 🚀 Next Steps

- Build a simple Streamlit dashboard for lenders
- Improve performance with techniques like SMOTE or XGBoost
- Deploy with Flask or FastAPI

---

## Author

**Vanessa Sandra Assesa**  
[GitHub: Assesa44](https://github.com/Assesa44)  
Email: veesandra30@gmail.com  


