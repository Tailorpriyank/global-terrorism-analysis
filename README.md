# 🧠 Employee Attrition Prediction Using Machine Learning

This project applies machine learning techniques to predict whether an employee is likely to leave a company, based on various workplace and personal attributes. By identifying key drivers of attrition such as overtime, job satisfaction, and income level, the model helps HR teams proactively address employee retention.

---

## 📊 Project Overview

- **Problem Statement**: Predict employee attrition using structured HR data.
- **Dataset**: IBM HR Analytics Employee Attrition Dataset
- **Objective**: Build a classification pipeline that accurately identifies employees at risk of leaving, and uncover the most influential features driving attrition.

---

## 🛠️ Tools & Technologies

- **Languages & Libraries**: Python, Pandas, NumPy, Seaborn, Matplotlib
- **ML Libraries**: Scikit-learn, XGBoost
- **Notebook Environment**: Jupyter Notebook

---

## 🧠 Key Steps

### 📥 1. Data Loading & Understanding
- Loaded the IBM HR dataset containing over 1,400 records.
- Assessed feature distributions, imbalance, and target variable proportions.

### 🧹 2. Data Cleaning & Preprocessing
- Encoded categorical variables using LabelEncoder.
- Dropped uninformative or redundant columns (`EmployeeNumber`, `Over18`, etc.).
- Checked for null values and ensured clean input for model training.

### 📊 3. Exploratory Data Analysis (EDA)
- Visualized attrition rates by:
  - Job satisfaction
  - Monthly income
  - Age
  - Work-life balance
  - Overtime status
- Used correlation heatmaps and boxplots to identify strong predictors.

### 🤖 4. Modeling & Evaluation
Models used:
- **Logistic Regression**
- **Random Forest Classifier**
- **XGBoost Classifier**

Metrics evaluated:
- Accuracy
- Confusion Matrix
- ROC Curve & AUC Score
- Feature Importance

---

## 📈 Results Summary

| Model               | Accuracy | Top Features                   |
|--------------------|----------|--------------------------------|
| Logistic Regression| ~83%     | Overtime, Age, Job Role        |
| Random Forest      | ~86%     | MonthlyIncome, JobLevel        |
| **XGBoost**        | **~89%** | OverTime, JobSatisfaction, Age |

- **XGBoost outperformed** other models in both accuracy and ROC-AUC.
- **OverTime** and **JobSatisfaction** were consistently top predictors across all models.

---


- Confusion Matrix
- ROC Curve
- Feature Importance (XGBoost)

---

## 📂 Repository Structure
📦P_Tailor_Final_Project
┣ 📄P_TAILOR_FINAL_PROJECT.ipynb  → Main notebook with all code
┣ 📄README.md                     → This file

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/Tailorpriyank/P_Tailor_Final_Project.git

cd P_Tailor_Final_Project
jupyter notebook P_TAILOR_FINAL_PROJECT.ipynb

💡 Final Takeaways
	•	XGBoost Classifier is most effective for this problem, achieving ~89% accuracy.
	•	Key attrition drivers:
	•	High Overtime
	•	Low Job Satisfaction
	•	Lower Monthly Income
	•	Younger Employees
	•	This model can help HR departments focus on early intervention for high-risk employees, saving on turnover costs and improving workplace engagement.

---
