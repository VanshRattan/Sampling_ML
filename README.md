# 📘 Sampling Assignment – Credit Card Fraud Detection  
**Student ID:** 102316118  

---

## 📌 Project Overview

This project analyzes how different **sampling techniques** affect the performance of
various **machine learning models** on a **highly imbalanced credit card fraud dataset**.

The main goal is to:
- Handle class imbalance correctly
- Apply multiple sampling techniques
- Train multiple ML models
- Compare results and identify the best sampling method

---

## 📂 Dataset Information

- **Dataset Name:** Creditcard_data.csv  
- **Source:**  
  https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv  
- **Target Column:** `Class`  
  - `0` → Normal Transaction  
  - `1` → Fraud Transaction  

The dataset is **highly imbalanced**, with fraud cases being very rare compared to normal transactions.

---

## ⚖️ Step 1: Data Balancing

Since the dataset is imbalanced, the minority class (fraud cases) was **oversampled**.

### What was done:
- Fraud records were randomly duplicated **with replacement**
- Oversampling continued until both classes had equal samples
- The dataset was shuffled to remove ordering bias

This step ensures fair learning for both classes.

---

## 🔄 Step 2: Sampling Techniques Used

After balancing the dataset, **five different sampling techniques** were applied:

| Sampling Code | Sampling Technique | Description |
|--------------|-------------------|-------------|
| Sampling1 | Simple Random Sampling | Random train-test split |
| Sampling2 | Stratified Sampling | Preserves class balance |
| Sampling3 | Bootstrap Sampling | Sampling with replacement |
| Sampling4 | K-Fold Sampling | Structured data splitting |
| Sampling5 | Stratified K-Fold Sampling | K-Fold with class balance |

Each sampling technique creates a different training and testing dataset.

---

## 🤖 Step 3: Machine Learning Models

Five machine learning models were trained on each sampled dataset:

| Model Code | Model Name |
|-----------|------------|
| M1 | Logistic Regression |
| M2 | K-Nearest Neighbors (KNN) |
| M3 | Decision Tree |
| M4 | Random Forest |
| M5 | Support Vector Machine (SVM) |

---

## 📊 Step 4: Model Evaluation

- Each model was trained on each sampled dataset
- Performance was evaluated using **Accuracy**
- Results were stored in a comparison table
- A bar graph was plotted for visual comparison

---

## 📈 Key Results

| Model | Best Sampling | Accuracy |
|-------|--------------|----------|
| Logistic Regression | Sampling4 | 97.47% |
| KNN | Sampling1 | 96.86% |
| Decision Tree | Sampling1 | 97.94% |
| Random Forest | Sampling1 | 97.65% |
| SVM | Sampling1 | 96.55% |

---

## 🏆 Best Sampling Technique

### ✅ Overall Best:
**Sampling1 – Simple Random Sampling**

- Performed best for **4 out of 5 models**
- Works effectively once the dataset is balanced
- Preserves the natural structure of the data

### ⚠️ Exception:
- **Logistic Regression** performed best with **Sampling4**
- Logistic Regression prefers cleaner and more structured data splits

---

## 🧠 Final Conclusion

The experiment shows that balancing the dataset is crucial before applying any sampling technique.
After balancing, **Simple Random Sampling** is sufficient and performs best for most machine learning
models. However, some models, such as Logistic Regression, benefit from more structured sampling
methods like K-Fold sampling.

This demonstrates that **there is no single sampling technique that is best for all models**,
and the choice of sampling method should depend on the model and data characteristics.

---

## 📁 Repository Structure

