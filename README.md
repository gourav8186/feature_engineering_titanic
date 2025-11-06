# 🧠 Feature Engineering Mini Project – Titanic Dataset

## 📘 Project Overview

This project demonstrates **Feature Engineering** using the **Titanic Dataset**.  
The main objective is to preprocess and transform the dataset using the four key stages of feature engineering — **Data Cleaning, Data Integration, Data Transformation, and Data Reduction** — without performing any model training.

---

## 🧩 Dataset Information

**Dataset Name:** Titanic Dataset  
**Source:** [Kaggle - Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)  
**Attributes:**

- PassengerId
- Survived (Target)
- Pclass
- Name
- Sex
- Age
- SibSp
- Parch
- Ticket
- Fare
- Cabin
- Embarked

---

## ⚙️ Steps Implemented

### 1️⃣ Data Cleaning

- Handled missing values using **median** for numeric and **mode** for categorical data.
- Removed duplicate rows.
- Detected and treated outliers using **IQR method**.

### 2️⃣ Data Integration

- Standardized column names (lowercase and underscores).
- Prepared for potential dataset merging using consistent naming.

### 3️⃣ Data Transformation

- Applied **Label Encoding** to low-cardinality categorical columns (e.g., Sex, Embarked).
- Applied **One-Hot Encoding** to multi-category columns.
- Scaled numeric columns using **StandardScaler**.
- Log-transformed skewed numeric data (e.g., Fare, Age).

### 4️⃣ Data Reduction

- Dropped irrelevant columns (Name, Ticket, Cabin).
- Removed highly correlated features (correlation > 0.9).
- Used **PCA (Principal Component Analysis)** to retain 95% of dataset variance.

---

## 📊 Output

After all four stages:

- The dataset is clean, normalized, and reduced.
- Final dataset saved as: `feature_engineered_titanic.csv`.
