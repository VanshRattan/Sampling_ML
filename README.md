# 📘 Sampling Assignment – Credit Card Fraud Detection
**Student ID:** 102316118

---

## 🎯 Quick Overview (1-Minute Summary)

**What:** Compare 5 sampling techniques across 5 ML models on a credit card fraud dataset.

**Why:** Dataset is imbalanced (fraud cases << normal cases). Need fair model training.

**How:** Balance data → Apply 5 sampling techniques → Train 5 models → Compare results.

---

## � The Process

```
1. Load Dataset           2. Balance Data           3. Apply 5 Sampling
   ↓                        ↓                         Techniques
   Imbalanced           Oversample Fraud              ↓
   (99.8% Normal)       (50-50 Split)            4. Train 5 Models
                                                     on Each Sample
                                                     ↓
6. Conclusion        5. Analyze Results        
   ↓                      ↓
Sampling1 BEST!    Results Table + Graph
(for 4/5 models)    Accuracy Comparison
```

---

## 📈 Key Results

| Model | Best Sampling | Accuracy |
|-------|--------------|----------|
| **Logistic Regression** | Sampling4 | 97.47% |
| **KNN** | Sampling1 | 96.86% |
| **Decision Tree** | Sampling1 | 97.94% |
| **Random Forest** | Sampling1 | 97.65% |
| **SVM** | Sampling1 | 96.55% |

**Winner:** Sampling1 (Simple Random) works best for 4/5 models! ⭐

---

## 🔄 5 Sampling Techniques Explained

| # | Technique | How It Works | Best For |
|---|-----------|-------------|----------|
| **1** | Simple Random | Random 75-25 split | Non-linear models, trees |
| **2** | Stratified | Split while keeping 50-50 ratio | Maintaining balance |
| **3** | Bootstrap | Sample with replacement | Reducing variance |
| **4** | K-Fold | Divide into 5 folds | Logistic Regression |
| **5** | Stratified K-Fold | K-Fold + balanced splits | Robust validation |

---

## 💡 Why Sampling1 Wins

✅ Data already balanced → No need for complex techniques  
✅ Simple = Fewer errors & faster  
✅ Works great with decision trees & random forests  
✅ Preserves natural data structure  

**Exception:** Logistic Regression prefers Sampling4 (K-Fold) for stable decision boundaries.

---

## 📁 Files

- `102316118.ipynb` – All code & experiments
- `Creditcard_data.csv` – Dataset
- `README.md` – This guide

---

## ✅ What We Learned

1. **Balance first** – Imbalanced data = biased models
2. **Simple > Complex** – When data is balanced, don't overcomplicate
3. **Model matters** – Linear vs non-linear models prefer different techniques
4. **No one-size-fits-all** – Test & choose based on your data & model type

**Final Takeaway:** For balanced datasets, use **Simple Random Sampling (Sampling1)** for best results with most ML models!

--  
