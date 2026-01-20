# 🧠 Adult Income Prediction Using Machine Learning

## 📌 Project Overview

This project predicts whether an individual earns more than $50K per year using demographic and socio-economic census data. The objective is to build and evaluate supervised machine learning models for income classification.

---

## 📂 Dataset

Dataset source:
https://huggingface.co/datasets/ETdanR/adult_income

Target classes:
- <=50K
- >=50K

---

## ⚙️ Machine Learning Models

- Logistic Regression
- Support Vector Machine (SVM)
- Random Forest

---

## 🧪 Data Preprocessing

- Handling missing values
- One-hot encoding for categorical variables
- Feature scaling using StandardScaler
- Train–validation split
- ColumnTransformer pipeline

---

## 📊 Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC–AUC Curve

---

## ▶️ How to Run

Install dependencies:

pip install pandas numpy scikit-learn matplotlib seaborn

Run notebook:

23048504 Prabin Kumar Gupta.ipynb

---

## 🎓 Academic Context

This project was developed as part of Artificial Intelligence coursework focusing on supervised learning and model evaluation.

---

## 📊 Results and Evaluation

The performance of three supervised machine learning models was evaluated using the validation dataset. 
Multiple evaluation metrics were used to ensure fair and reliable comparison, including Accuracy, Precision, Recall, F1-score, Confusion Matrix, and ROC–AUC.

---

### 🔍 Evaluation Metrics Used

- **Accuracy** – Overall correctness of predictions  
- **Precision** – Correctness of positive income predictions  
- **Recall** – Ability to identify high-income individuals  
- **F1-score** – Balance between precision and recall  
- **Confusion Matrix** – Distribution of true/false predictions  
- **ROC–AUC Curve** – Model discrimination capability  

---

### 🧪 Model-wise Performance Summary

| Model | Accuracy | ROC–AUC |
|------|----------|---------|
| Logistic Regression | 0.80 | 0.887 |
| Support Vector Machine (SVM) | 0.81 | 0.890 |
| Random Forest | 0.80 | 0.886 |

---

### 📌 Confusion Matrix Summary

- **Logistic Regression**
  - Balanced prediction between income classes
  - Interpretable and stable performance

- **Support Vector Machine**
  - Slightly higher recall for high-income class (>50K)
  - Best overall classification balance

- **Random Forest**
  - Strong non-linear learning capability
  - Comparable performance but slightly higher variance

---

### 📈 ROC Curve Analysis

- All three models achieved **ROC–AUC values above 0.88**
- Indicates strong discriminative power between income classes
- The **SVM model achieved the highest ROC–AUC**, suggesting better boundary separation

---

### 🏆 Best Performing Model

Based on experimental results:

- **Support Vector Machine (SVM)** achieved the best overall performance
- Highest ROC–AUC score
- Balanced precision and recall
- Suitable for structured tabular income prediction problems

---

### ✅ Key Observations

- Feature preprocessing significantly improved model performance
- Log-transformation reduced skewness in capital-gain and capital-loss features
- One-hot encoding effectively handled categorical variables
- Classical machine learning models remain competitive for structured census data

---

These results demonstrate that traditional supervised learning algorithms, when properly preprocessed and evaluated, can provide reliable and interpretable predictions for income classification tasks.


## 👨‍💻 Author

Prabin Kumar Gupta



