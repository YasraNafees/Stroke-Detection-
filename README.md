# 🏥 Stroke Risk Prediction using Machine Learning

Predicts stroke risk using patient health metrics and lifestyle factors.

![Python](https://img.shields.io/badge/Python-3.x-blue)
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
