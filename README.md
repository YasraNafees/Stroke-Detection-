# 🏥 Stroke Risk Prediction using Machine Learning

Predicts stroke risk using patient health metrics and lifestyle factors.

![Python](https://img.shields.io/badge/Python-3.x-blue)a# 🧠 Stroke Detection Predictive Model

![Python](https://img.shields.io/badge/Python-3.10+-blue) ![GradientBoosting](https://img.shields.io/badge/GradientBoosting-Enabled-orange) ![Accuracy](https://img.shields.io/badge/Accuracy-72%25-yellow) ![AUC](https://img.shields.io/badge/AUC-0.72-yellowgreen) ![License](https://img.shields.io/badge/License-MIT-yellow)

### Gradient Boosting Classifier | 10,000 Records | SMOTE Balancing | Clinical Risk Factors

A machine learning model that predicts stroke risk using clinical and demographic data. Built with Gradient Boosting and SMOTE oversampling to handle class imbalance across 10,000 patient records.

---

## 📊 Model Performance

| Metric | Score |
|---|---|
| Accuracy | 72% |
| AUC-ROC | 0.72 |
| Precision (Stroke) | 0.52 |
| Recall (Stroke) | 0.70 |
| F1-Score (Stroke) | 0.60 |

---

## ✨ Key Features

- **Gradient Boosting Classifier:** 200 estimators, learning rate 0.05, max depth 5 — tuned to reduce overfitting.
- **SMOTE Oversampling:** Balanced class distribution from 70/30 to 50/50 for unbiased training.
- **Socioeconomic Status (SES):** Unique feature inclusion — captures social determinants of stroke risk often ignored in standard datasets.
- **Comprehensive EDA:** Age distribution, gender analysis, SES vs stroke, diabetes vs stroke correlation analysis.
- **Model Persistence:** Saved via `joblib` for production deployment.

---

## 🔍 Top Predictive Features

1. **Age** — Strongest predictor (correlation: 0.36)
2. **Hypertension** — Second strongest (correlation: 0.39)
3. **Heart Disease** — Significant comorbidity (correlation: 0.27)
4. **Avg Glucose** — Metabolic risk factor (correlation: 0.22)
5. **Diabetes** — Compounding risk factor (correlation: 0.25)

---

## 🛠️ Tech Stack

| Component | Tool |
|---|---|
| Language | Python 3.10+ |
| ML Framework | Scikit-Learn |
| Boosting | Gradient Boosting Classifier |
| Imbalance Handling | SMOTE (imbalanced-learn) |
| Data Processing | Pandas, NumPy |
| Visualization | Matplotlib, Seaborn |
| Model Export | Joblib |

---

## 📁 Dataset

- **Records:** 10,000 patients
- **Features:** 9 clinical + demographic attributes
- **Target:** Binary (0 = No Stroke, 1 = Stroke)
- **Class Distribution:** 70% No Stroke, 30% Stroke
- **Missing Values:** None

---

## 🚀 Quick Start

**1. Clone the repo:**
```bash
git clone https://github.com/YasraNafees/stroke-detection.git
cd stroke-detection
```

**2. Install dependencies:**
```bash
pip install -r requirements.txt
```

**3. Run the notebook:**
```bash
jupyter notebook stroke_detection.ipynb
```

**4. Load saved model:**
```python
import joblib
import pandas as pd

model = joblib.load('Gradient boosting Stroke Model.pkl')

new_data = pd.DataFrame({
    'Age': [72],
    'Gender': [1],
    'SES': [2],
    'Hypertension': [1],
    'Heart_Disease': [1],
    'BMI': [28.5],
    'Avg_Glucose': [130.0],
    'Diabetes': [1],
    'Smoking_Status': [0]
})

prediction = model.predict(new_data)
print("Stroke Prediction:", "High Risk" if prediction[0] == 1 else "Low Risk")
```

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.
![Model](https://img.shields.io/badge/Model-Gradient%20Boosting-orange)
![Accuracy](https://img.shields.io/badge/Accuracy-72%25-yellow)

---

## 📌 Overview

Classifies individuals as at-risk or not-at-risk for stroke using health
indicators like age, BMI, glucose level, and smoking status.

---

## 📊 Dataset Features

`Age` `Hypertension` `Heart Disease` `BMI` `Smoking Status` `Glucose Level`

---

## 🤖 Model Performance

**Gradient Boosting Classifier**

| Metric | Score |
|--------|-------|
| Accuracy | 72% |
| AUC Score | 0.72 |

**Confusion Matrix**

| | Predicted No | Predicted Yes |
|---|---|---|
| **Actual No** | 1035 (TN) | 378 (FP) |
| **Actual Yes** | 174 (FN) | 413 (TP) |

---

## 🛠 Tech Stack

`Python` `Scikit-learn` `Pandas` `NumPy` `Seaborn` `Matplotlib`

---

## ▶️ How to Run
```bash
git clone https://github.com/YasraNafees/Stroke-Detection-
pip install -r requirements.txt
jupyter notebook
```

---

## 📄 License
MIT — open source and free to use.
