#### Name - Yashraj Ramdas Chavan  
#### Roll No. - DA25M031  
#### Assignment 7 - Data Analytics Lab (DA5401) JUL–NOV 2025  

# 🧠 DA5401 — Assignment 7: Model Selection using ROC & PRC

### 📘 Overview
This assignment explores **model selection and evaluation** using **Receiver Operating Characteristic (ROC)** and **Precision–Recall (PRC)** curves on the **Landsat Satellite dataset**.  
The task involves comparing multiple classifiers in a **multi-class classification** setting, analyzing their performance beyond simple accuracy.

---

### 🎯 Objective
To apply and interpret **ROC-AUC** and **Precision–Recall (PRC)** curves for evaluating models on a complex multi-class dataset.  
The focus is on understanding how strong and weak classifiers behave across thresholds.

---

### ⚙️ Models Evaluated
- **KNN (K-Nearest Neighbors)**  
- **SVC (Support Vector Classifier)**  
- **Decision Tree**  
- **Logistic Regression**  
- **RandomForest Classifier**  
- **XGBoost Classifier**  
- **Dummy (prior)**
- **Dummy (stratified)**

---

### 📊 Key Metrics
Each model was evaluated on:
- **Accuracy**
- **Weighted F1-Score**
- **Macro ROC-AUC**
- **Average Precision (PRC-AP)**

---

### 📈 Results Summary
| Model | Accuracy | Weighted F1 | ROC-AUC | PRC-AP |
|:------|----------:|------------:|--------:|-------:|
| **XGBoost** | 0.903 | 0.900 | **0.987** | **0.937** |
| **RandomForest** | 0.895 | 0.890 | 0.985 | 0.930 |
| **SVC** | 0.880 | 0.875 | 0.981 | 0.902 |
| **KNN** | 0.893 | 0.892 | 0.974 | 0.896 |
| **Logistic Regression** | 0.852 | 0.843 | 0.974 | 0.867 |
| **Decision Tree** | 0.830 | 0.828 | 0.883 | 0.688 |
| **Dummy (prior)** | 0.241 | 0.094 | 0.500 | 0.167 |
| **Dummy (stratified)** | 0.194 | 0.194 | **0.497** | 0.168 |

---

### 🔍 Insights
- **XGBoost** achieved the best overall performance across all metrics.  
- **RandomForest** and **SVC** followed closely with strong generalization.  
- **Dummy (stratified)** model demonstrated **AUC < 0.5**, representing random or worse-than-random classification.
- ROC and PRC analyses revealed that curve-based evaluation provides deeper insights than accuracy alone.

---

### 🧠 Key Learning
This assignment highlights how **curve-based evaluation (ROC & PRC)** provides a more reliable picture of model performance, especially in **imbalanced or multi-class** scenarios.  

---

