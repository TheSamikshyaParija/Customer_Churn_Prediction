# 📈 Customer Churn Prediction Using Logistic Regression

## 🧠 Overview

This project aims to predict **customer churn** — whether a customer is likely to stop using a service — using a **Logistic Regression** model. The notebook includes a complete data science pipeline from preprocessing to model evaluation, focusing on insights gained through Exploratory Data Analysis (EDA) and feature engineering.

---

## 📂 Dataset

- **Source:** IBM Telco Customer Churn dataset  
- **Download URL:**  
  https://raw.githubusercontent.com/IBM/telco-customer-churn-on-icp4d/master/data/Telco-Customer-Churn.csv

The dataset contains customer demographic information, account details, and service usage behavior. The target variable is `Churn`.

---

## 🧰 Libraries Used

- `pandas`, `numpy` — data handling and manipulation
- `matplotlib`, `seaborn` — data visualization
- `scikit-learn` — machine learning and preprocessing

---

## 🚦 Workflow Summary

### 1. **Environment Setup**
   - Required packages are installed using pip.
   - Common libraries such as `pandas`, `numpy`, `matplotlib`, `seaborn`, and `sklearn` are imported.

### 2. **Data Loading**
   - Data is loaded from a public GitHub repository.
   - The dataset is saved locally for reuse.
   - Initial inspection using `.head()` and `.info()`.

### 3. **Data Cleaning**
   - Conversion of `TotalCharges` from string to numeric with error coercion.
   - Handling missing values using median imputation.
   - Dropping irrelevant columns (e.g., `customerID`).
   - Label encoding of binary categorical features.

### 4. **Exploratory Data Analysis (EDA)**
   - Visualizations:
     - **Countplots** for churn distribution.
     - **Contract type vs churn** analysis.
     - **Boxplots** for Monthly Charges vs churn.
   - EDA helps in understanding the data distribution and spotting key churn indicators.

### 5. **Preprocessing**
   - Label Encoding of binary variables like `Yes/No`, `Male/Female`.
   - Train-test split (75-25%).
   - Standardization using `StandardScaler`.

### 6. **Modeling**
   - **Logistic Regression** is used as the classification model.
   - Model is trained on standardized features.

### 7. **Evaluation**
   - Metrics used:
     - Accuracy Score
     - Confusion Matrix
     - Classification Report (Precision, Recall, F1-score)
   - Results demonstrate how well the model predicts churn.

--
### Author : Samikshya Parija
### Institution : Siksha 'O' Anusandhan 
