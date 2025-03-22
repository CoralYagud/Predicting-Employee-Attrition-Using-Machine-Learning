# Predicting-Employee-Attrition-Using-Machine-Learning
 The analysis revealed critical factors influencing employee attrition, including age, monthly income, and overtime.

 # 📉 Employee Attrition Prediction Using Machine Learning

## 👥 Project Overview

This project aims to predict employee attrition (i.e., whether an employee will leave a company) using machine learning techniques. By analyzing various employee attributes such as demographics, work experience, and job satisfaction, we identify key factors influencing attrition and build predictive models to help organizations improve retention strategies.

This research was conducted by:  
**Lior Biton, Coral Yagud, Naama Maimon, Stav Barak**

---

## 🎯 Research Question

**What are the main factors leading to employee attrition in large companies?**

---

## 🧠 Key Insights

- Employees who are younger, have lower monthly income, or work overtime are more likely to leave.
- XGBoost showed the best predictive performance among tested models.
- SHAP values provided clear interpretability for feature importance.

---

## 📁 Dataset

**IBM HR Analytics Employee Attrition & Performance Dataset**  
- Source: [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)  
- Records: 1,470 employees  
- Features: 35 columns including age, income, job role, department, overtime, satisfaction levels, etc.

---

## 🧹 Data Preparation

- No missing values or duplicates.
- Categorical variables encoded.
- Binary labels used for `Attrition` and `OverTime`.
- Irrelevant columns dropped (e.g., EmployeeNumber, StandardHours).

---

## 🔎 Exploratory Data Analysis (EDA)

Visualizations revealed:
- High attrition among younger employees (age 20–35).
- Lower income correlates with higher attrition.
- Overtime and low job satisfaction significantly increase attrition risk.
- No significant attrition difference between genders.

---

## 🧪 Models Used

We trained and evaluated three models:

| Model              | Accuracy | Best For                          |
|-------------------|----------|-----------------------------------|
| Logistic Regression | 87.07%  | Baseline + High interpretability |
| Random Forest       | 86.39%  | Handling complex data patterns   |
| XGBoost             | 87.30%  | Best overall performance         |

👉 All models were trained using a **70-30 train-test split**.

---

## 📊 SHAP Analysis – Feature Importance

Top factors increasing attrition:
- **OverTime**
- **Age (younger employees)**
- **Monthly Income (lower range)**
- **Stock Option Level**
- **Number of Companies Worked**
- **Distance From Home**

> SHAP values helped make the model transparent and explainable for HR stakeholders.

---

## 🗂️ Project Structure


---

## 🚀 How to Run

### 📦 Requirements

Install required Python packages:

```bash
pip install pandas matplotlib seaborn scikit-learn xgboost shap

