# 🧠 Stroke Risk Prediction using Machine Learning

## 📌 Overview
This project develops a machine learning model to predict the likelihood of stroke using demographic and clinical data. 

Stroke is one of the leading causes of mortality globally and in the Philippines. Early identification of high-risk individuals can support preventive healthcare strategies and improve patient outcomes.

---

## 🎯 Objectives
- Identify key risk factors associated with stroke
- Perform exploratory data analysis (EDA) to uncover patterns
- Build and compare multiple machine learning models
- Evaluate model performance using appropriate metrics
- Assess ethical considerations and potential biases

---

## 📊 Dataset
- Source: Kaggle — Stroke Prediction Dataset  
- Records: 5,000+ patients  
- Features include:
  - Age
  - Hypertension
  - Heart disease
  - BMI
  - Smoking status
  - Average glucose level

---

## ⚙️ Methodology

### 1. Data Preprocessing
- Handled missing BMI values using median imputation
- Encoded categorical variables using one-hot encoding
- Standardized numerical features
- Addressed class imbalance using SMOTE

### 2. Exploratory Data Analysis
- Identified strong relationships between stroke and:
  - Age
  - Glucose levels
  - Hypertension
- Observed significant class imbalance

### 3. Feature Engineering
- Created derived features (e.g., cardiovascular risk score)
- Applied feature selection techniques
- Performed PCA for dimensionality analysis

### 4. Model Implementation
Models evaluated:
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)

Evaluation metrics:
- Accuracy
- Precision
- Recall
- F1 Score
- ROC AUC

---

## 📈 Results

| Model | Accuracy | Recall | ROC AUC |
|---|---|---|---|
Logistic Regression | 0.75 | **0.80** | **0.84** |
Random Forest | **0.92** | 0.18 | 0.76 |
SVM | 0.81 | 0.54 | 0.78 |

### Key Insights
- Logistic Regression achieved the highest recall, making it more suitable for detecting stroke cases
- Random Forest achieved high accuracy but failed to identify most stroke cases
- Stroke prediction involves multiple interacting variables rather than a single dominant factor

---

## ⚖️ Ethical Considerations
- High risk of **false negatives** (missed stroke cases)
- Class imbalance introduces prediction bias
- Model should be used as a **decision-support tool**, not a standalone diagnostic system
- Important to ensure fairness across patient groups

---

## 🛠️ Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib, Seaborn

---

## 📁 Project Structure
├── notebooks/
│   └── Baquiran_LorenzoCarlos_Pillar5_Capstone.ipynb
├── data/
│   └── healthcare_dataset_stroke_data.csv
├── models/
├── images/
├── README.md
├── requirements.txt
