
# Linear & Logistic Regression Project

## Dataset
The dataset `Admission.csv` contains various features of student profiles aimed at predicting the likelihood of admission to a university.

---

## 1. Project Objectives

### 1. Exploratory Data Analysis (EDA)
- Load and inspect the dataset.
- Plot distributions of selected features.
- Use `pairplot` to identify the most highly correlated pair of features.

### 2. Linear Regression (Closed-Form)
- Define `GRE Score` as the target variable.
- Use other columns as input features.
- Preprocess the data (handle missing values, normalize).
- Split into training/testing sets (e.g., 80/20).
- Apply the closed-form solution for linear regression:
  ```
  w = (XᵀX)⁻¹ Xᵀy
  ```
- Report **Mean Squared Error (MSE)** on both sets.

### 3. Theoretical Analysis
- Discuss pros/cons of using closed-form solutions.
- Explain why gradient-based methods are often preferred in practical applications.

### 4. Regularization Impact
- Use **Ridge Regression (L2)** and **Lasso Regression (L1)** using built-in functions.
- Compare learned coefficients in both models.
- Analyze whether the behavior aligns with theoretical expectations.

### 5. Logistic Regression (Manual Implementation)
- Create a new binary column `Admission`:
  - `1` if `Chance of Admit > 0.5`, else `0`.
- Drop `Chance of Admit` column.
- Set `Admission` as target; others as features.
- Implement **Logistic Regression using Newton-Raphson optimization**.
- Do not use library-based logistic regression.
- Report accuracy and confusion matrix on both training and testing sets.

### 6. Coefficient Analysis
- Analyze which feature had the most influence on admission.
- Compare with EDA findings (from `pairplot`) to check consistency.

---

## Learning Goals
- Understand and implement different regression models.
- Gain experience in data preprocessing, mathematical modeling, and evaluation.
- Learn the impact of regularization techniques on model simplicity and performance.

---
