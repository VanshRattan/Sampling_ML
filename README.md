# 📘 Sampling Assignment – Credit Card Fraud Detection  
**Student ID:** 102316118  

---

## 📌 Overview

This project evaluates how different **sampling techniques** affect the performance of
multiple **machine learning models** on an **imbalanced credit card fraud dataset**.

**Goals:**
- Handle class imbalance
- Apply different sampling techniques
- Compare model performance
- Identify the best sampling method

---

## 🔁 Workflow


![alt text](image.png)

---

## ⚖️ Data Balancing

The dataset was highly imbalanced.  
The minority class (fraud cases) was **oversampled with replacement** until both classes were equal.
The balanced dataset was shuffled to avoid bias.

---

## 🔄 Sampling Techniques

| Code | Technique |
|-----|----------|
| Sampling1 | Simple Random Sampling |
| Sampling2 | Stratified Sampling |
| Sampling3 | Bootstrap Sampling |
| Sampling4 | K-Fold Sampling |
| Sampling5 | Stratified K-Fold Sampling |

---

## 🤖 Machine Learning Models

Logistic Regression, KNN, Decision Tree, Random Forest, and SVM were used for evaluation.

---

## 📈 Key Results

| Model | Best Sampling | Accuracy |
|------|--------------|----------|
| Logistic Regression | Sampling4 | 97.47% |
| KNN | Sampling1 | 96.86% |
| Decision Tree | Sampling1 | 97.94% |
| Random Forest | Sampling1 | 97.65% |
| SVM | Sampling1 | 96.55% |

---

## 🏆 Best Sampling Technique

- **Overall Best:** Sampling1 (Simple Random Sampling)  
- **Exception:** Logistic Regression performs best with Sampling4  

---

## 🧠 Conclusion

After balancing the dataset, **Simple Random Sampling** worked best for most models.
Logistic Regression benefited from **K-Fold Sampling** due to its sensitivity to data splits.
This shows that the best sampling technique depends on the model.

---
