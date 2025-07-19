# 📊 Jane Street Market Prediction

> Capstone project developed as part of my Master's in Business Analytics at California State University – East Bay.

This project addresses the Kaggle competition hosted by Jane Street, a quantitative trading firm. The challenge involves building a machine learning model to predict whether a trade should be executed (action = 1) or not (action = 0) based on a high-dimensional, anonymized financial dataset.

---

## 📁 Project Files

| File | Description |
|------|-------------|
| `JaneStreetMarketPrediction-Final.ipynb` | Final notebook containing preprocessing, feature selection, model training & evaluation |
| `Capstone_Report.pdf` | Full technical report |
| `Jane_Street_Presentation.pdf` | Presentation slides prepared for academic defense |

---

## 🔍 Problem Overview

- **Dataset size**: 6 GB
- **Rows**: 2.3M+, **Features**: 138 (anonymized)
- **Target**: `action` → 1 (trade) or 0 (pass)

Approaches:
- **Approach 1**: If `resp > 0` then action = 1 else 0
- **Approach 2**: If `(resp * weight)` & `(resp_1 * weight)` & ... > 0 then action = 1 else 0

---

## 🛠️ Technologies Used

- Python, Pandas, NumPy, Matplotlib
- Scikit-learn, Random Forest, MLPClassifier
- Data preprocessing, EDA, Feature Engineering
- Evaluation: Confusion Matrix, Accuracy

---

## ✅ Key Results

| Model | Approach 1 | Approach 2 |
|-------|------------|------------|
| MLP (Neural Net) | 50.23% | **73.53%** ✅ |
| Decision Tree | 59.98% | 62.42% |
| Random Forest | 52.13% | **73.53%** ✅ |

🔎 **Best Model**: Multiple Layer Perceptron using Approach 2 (accuracy: 73.53%)

---

## 🧠 Learnings & Challenges

- Heavy preprocessing required due to large (6 GB) dataset.
- Feature selection was complex due to anonymized features and multicollinearity.
- Future work includes running the pipeline on AWS for better scalability.

---

## 📎 References

- [Kaggle Competition](https://www.kaggle.com/c/jane-street-market-prediction)
- Feature selection via Random Forest, SHAP
- Various supporting notebooks and documentation (see report)

---

## 🙋‍♀️ Author

**Prathyusha Sathineni**  
✉️ [sai.prathyusha08@gmail.com](mailto:sai.prathyusha08@gmail.com)  
🔗 [LinkedIn](https://www.linkedin.com/in/prathyushasathineni)

---
