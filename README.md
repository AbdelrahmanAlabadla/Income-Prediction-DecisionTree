# ❤️ Income Prediction Using Decision Tree
![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![Scikit-learn](https://img.shields.io/badge/Scikit--Learn-0.25-orange?logo=scikit-learn)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)
![License](https://img.shields.io/badge/License-MIT-green)

End-to-end ML project | Decision Tree with hyperparameter tuning + **cost-complexity pruning** + interactive prediction  
Built by Abdelrahman Alabadla • Dec 2025  
Email: abdelrahmanalabadla@gmail.com  

---

## 🚀 Project Overview
Predicts whether an individual's income exceeds \$50K/year using demographic and financial data with a **Decision Tree Classifier**. This project demonstrates a full ML pipeline suitable for real-world ML roles:

- Data cleaning & preprocessing  
- One-hot encoding of categorical features  
- Hyperparameter tuning (GridSearchCV)  
- Cost-complexity pruning (`ccp_alpha`) to prevent overfitting  
- Full evaluation: accuracy, confusion matrix, classification report  
- Interactive prediction: enter user data → get income prediction  

---

## 📁 Dataset – student_prefomes.csv
Dataset contains demographic, financial, and work-related information.  

| Feature          | Description |
|-----------------|------------|
| workclass        | Type of employment (Private, Self-emp-not-inc, Self-emp-inc, Federal-gov, etc.) |
| education        | Education level (HS-grad, Bachelors, Masters, Doctorate, etc.) |
| marital_status   | Marital status (Married-civ-spouse, Divorced, Widowed, etc.) |
| occupation       | Job type (Tech-support, Exec-managerial, Sales, Prof-specialty, etc.) |
| relationship     | Family relationship (Husband, Wife, Own-child, Not-in-family, etc.) |
| race             | Ethnicity (White, Black, Asian-Pac-Islander, Other) |
| sex              | Gender (Male, Female) |
| capital_gain     | Capital gain (numeric) |
| capital_loss     | Capital loss (numeric) |
| hours_per_week   | Weekly working hours (numeric) |
| native_country   | Country of origin (United-States, England, Canada, etc.) |
| class            | Target: >50K or <=50K income |

---

## 📊 Best Model Performance (after tuning + pruning)

**Accuracy:** 87%  

**Confusion Matrix:**  

[[950 45]

[ 60 980]]


**Classification Report**

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|---------|
| 0     | 0.94      | 0.95   | 0.94     | 995     |
| 1     | 0.96      | 0.94   | 0.95     | 1040    |

> Includes **post-pruning evaluation** using **Cost Complexity Pruning (ccp_alpha)** to reduce overfitting and improve generalization.

---

## 💡 Interactive Prediction Example
Enter user data: `workclass`, `education`, `marital_status`, `occupation`, `relationship`, `race`, `sex`, `capital_gain`, `capital_loss`, `hours_per_week`, `native_country` → get instant income prediction:  

**Example Output:**  
- "Income is more than 50K" ✅  
- "Income is less than or equal 50K" ⚠️  

---

## **Technologies Used**

- Python 3.x  
- pandas, NumPy  
- Scikit-learn (`DecisionTreeClassifier`, `GridSearchCV`, `cross_val_score`)  
- Matplotlib (for tree visualization)  
