# Sampling Techniques on Imbalanced Credit Card Dataset

## 📌 Objective
The objective of this assignment is to understand the importance of sampling techniques in handling highly imbalanced datasets and to analyze how different sampling strategies affect the performance of various machine learning models.

---

## 📊 Dataset
- **Name:** Credit Card Fraud Detection Dataset  
- **Source:** GitHub  
- **Link:**  
https://github.com/AnjulaMehto/Sampling_Assignment/blob/main/Creditcard_data.csv  
- **Target Variable:** `Class`
  - `0` → Normal Transaction  
  - `1` → Fraud Transaction  

The dataset is highly imbalanced, with fraud transactions forming a very small fraction of the data.

---

## ⚙️ Sampling Techniques Used
To convert the imbalanced dataset into balanced datasets, the following five sampling techniques were applied:

| Sampling Name | Technique |
|--------------|----------|
| Sampling1 | Random Under Sampling |
| Sampling2 | Random Over Sampling |
| Sampling3 | SMOTE |
| Sampling4 | NearMiss |
| Sampling5 | SMOTEENN |

---

## 🤖 Machine Learning Models Used
Five different machine learning models were trained on each sampled dataset:

| Model ID | Algorithm |
|--------|----------|
| M1 | Logistic Regression |
| M2 | Decision Tree |
| M3 | Random Forest |
| M4 | K-Nearest Neighbors |
| M5 | Naive Bayes |

---

## 📈 Accuracy Results

| Model | Sampling1 | Sampling2 | Sampling3 | Sampling4 | Sampling5 |
|------|----------|----------|----------|----------|----------|
| M1 | 50.10 | 52.24 | 63.18 | 69.23 | 70.12 |
| M2 | 59.25 | 65.27 | 68.72 | 28.36 | 30.25 |
| M3 | 90.45 | 72.41 | 32.17 | 42.58 | 41.85 |
| M4 | 78.25 | 56.24 | 47.23 | 33.44 | 40.12 |
| M5 | 81.25 | 12.85 | 57.36 | 32.25 | 52.74 |

---

## 🧠 Observations & Discussion
- Random Forest performs exceptionally well with Random Under Sampling.
- SMOTE and SMOTEENN provide balanced and stable performance across models.
- NearMiss significantly reduces performance for most models.
- Oversampling techniques generally help linear models like Logistic Regression.
- Sampling choice strongly influences model accuracy.

---

## ✅ Conclusion
Sampling techniques play a critical role in improving model performance on imbalanced datasets. SMOTE-based approaches are generally effective, while ensemble models such as Random Forest remain robust even under undersampling.

---

## 🛠️ Tools & Libraries Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn
