# 🛡️ Fraud Detection Using Machine Learning

## 📌 Project Overview
This project focuses on detecting fraudulent financial transactions using machine learning. Fraud detection is a **security domain problem** involving highly imbalanced data where fraudulent cases are extremely rare. The objective is to build a model that can effectively identify fraud while maintaining a balance between precision and recall.

---

## 🎯 Problem Statement
Financial fraud causes major economic losses worldwide. Detecting fraud is challenging because:
- Fraud cases are **very rare (<0.5%)**
- Data is highly imbalanced
- Fraud patterns change over time

This project builds an intelligent model to detect suspicious transactions using behavioral and transactional features.

---

## 📊 Dataset Information
- Domain: **Security / Fraud Detection**
- Records: **500,000+ transactions**
- Features: **20+ attributes**
- Fraud Rate: ~0.4%
- Dataset satisfies capstone requirements (large scale & multi-feature)

---

## ⚙️ Techniques Used

### 🔹 Data Preprocessing
- Handling missing values
- Feature scaling
- Train–test split

### 🔹 Feature Engineering
- Transaction hour extraction
- Log transformation of transaction amount
- Distance between customer and merchant location
- User spending behavior features
- Merchant risk score

### 🔹 Handling Class Imbalance
- Used `scale_pos_weight` in XGBoost
- Threshold tuning
- Evaluation using **PR-AUC** instead of accuracy

### 🔹 Model Used
**XGBoost Classifier** — effective for structured/tabular data and imbalanced datasets.

---

## 📈 Model Performance

| Metric | Score |
|------|------|
| ROC-AUC | **0.96** |
| PR-AUC | **0.24** |
| Recall (Fraud) | **0.66** |
| Precision (Fraud) | **0.13** |
| F1 Score | **0.22** |

➡ The model performs **~60× better than random guessing** for fraud detection.

---

## 📉 Visualizations
- Confusion Matrix  
- ROC Curve  
- Precision–Recall Curve  
- Feature Importance Plot  

These visualizations help in understanding model performance and feature impact.

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
