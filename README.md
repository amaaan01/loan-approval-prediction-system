# 💰 Loan Approval Prediction using Machine Learning

## 📌 Project Overview

Banks receive thousands of loan applications every day. Manually reviewing each application is time-consuming and can lead to inconsistencies.

This project uses Machine Learning to predict whether a loan application will be approved or rejected based on applicant financial, personal, employment, and loan-related information.

The goal is to automate the loan approval process and assist banks in making faster and more consistent decisions.

---

## 🎯 Problem Statement

Can we predict whether a loan applicant will be approved or rejected using historical applicant data?

This is a binary classification problem where:

* Approved = 1
* Rejected = 0

---

## 📊 Dataset Information

Dataset Size:

* 1,000 Applicants
* 19 Features

### Features Include

#### Financial Information

* Income
* Credit Score
* Debt-to-Income Ratio (DTI)
* Savings Balance
* Loan Amount

#### Personal Information

* Age
* Gender
* Marital Status
* Dependents
* Education

#### Employment Information

* Employment Status
* Employer Category

#### Loan Information

* Loan Purpose
* Loan Term
* Property Area
* Collateral

Target Variable:

* Loan Approved

---

## ⚙️ Data Preprocessing

The following preprocessing steps were performed:

### Missing Value Handling

* Numerical Features → Mean Imputation
* Categorical Features → Mode Imputation

### Encoding

* Label Encoding
* One-Hot Encoding

### Feature Scaling

* StandardScaler

### Feature Engineering

Additional features were created:

* DTI_Ratio²
* Credit_Score²

These engineered features helped capture non-linear relationships within the data.

---

## 🤖 Machine Learning Models

Three classification models were implemented and compared:

### 1. Logistic Regression

* Fast and interpretable
* Works well for binary classification

### 2. K-Nearest Neighbors (KNN)

* Distance-based algorithm
* Sensitive to feature scaling

### 3. Naive Bayes

* Probabilistic classifier
* Fast training and prediction

---

## 📈 Results

### Baseline Models

| Model               | Accuracy | F1 Score |
| ------------------- | -------- | -------- |
| Logistic Regression | ~82%     | ~0.75    |
| KNN                 | ~79%     | ~0.71    |
| Naive Bayes         | ~75%     | ~0.66    |

### After Feature Engineering

| Model               | Accuracy | F1 Score |
| ------------------- | -------- | -------- |
| Logistic Regression | ~84%     | ~0.78    |
| KNN                 | ~81%     | ~0.74    |
| Naive Bayes         | ~77%     | ~0.69    |

🏆 Best Model: Logistic Regression

---

## 🔍 Key Findings

* Feature engineering improved all models.
* Credit Score and DTI Ratio were strong predictors.
* Logistic Regression consistently achieved the best performance.
* Evaluating only accuracy is not enough for imbalanced datasets.
* F1 Score provides a better measure of classification performance.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Seaborn
* Matplotlib

---

## 📂 Project Structure

```text
loan-approval-prediction-ml/
│
├── loan_approval_data.csv
├── ML_LoanApproval_Mini_Project.ipynb
├── loan_approval.pdf
├── README.md
```

---

## 📚 Key Learnings

Through this project, I gained hands-on experience with:

* Data Cleaning
* Feature Engineering
* Classification Algorithms
* Model Evaluation
* Handling Imbalanced Data
* Machine Learning Pipelines

---

## 🚀 Future Improvements

* Hyperparameter Tuning
* Cross Validation
* Ensemble Models
* XGBoost
* Model Deployment using Flask/FastAPI
* MLOps Integration

---

## 👨‍💻 Author

Amaan Shaikh

Aspiring Data Science Engineer | Machine Learning Enthusiast

Feel free to connect and share feedback!
