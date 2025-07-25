# 🔍 UNSW-NB15 Cyber Attack Detection using Machine Learning

This project applies various machine learning algorithms to detect cyber attacks based on the UNSW-NB15 dataset. The dataset includes both normal and attack network traffic data, and the project focuses on binary classification (normal vs attack).

> 🎓 **This is the final project for the Summer Internship at NTI - Machine Learning Track.**

---

## 📂 Project Structure

```
📁 Final Evaluation Project/
│
├── UNSW_NB15_training-set.csv
├── UNSW_NB15_testing-set.csv
├── UNSW_NB15___Cybersecurity_Threat_Detection.ipynb
└── README.md
```

---

## 📌 Objective

To build and evaluate multiple ML models that classify network connections as either:
- 🟢 **Normal (label = 0)**
- 🔴 **Attack (label = 1)**

---

## 📊 Dataset Overview

- The dataset contains a mix of numerical and categorical features such as:
  - `proto`, `service`, `state`, `dur`, `sbytes`, `dbytes`, etc.
- It also contains:
  - `label` (target)
  - `attack_cat` (multiclass attack category)

---

## 🔧 Preprocessing Steps

- ✅ Dropped duplicates & checked for nulls  
- ✅ Label encoding for `proto`, `service`, `state`  
- ✅ Feature scaling using `StandardScaler`  
- ✅ Feature correlation matrix analysis  
- ✅ Dimensionality reduction using PCA (retaining 95% variance)  
- ✅ SMOTE used to handle class imbalance in training set  

---

## 📚 Machine Learning Models Applied

| Model                | Description                  |
|---------------------|------------------------------|
| KNN                 | With optimized `k` value     |
| Logistic Regression | Baseline model               |
| Decision Tree       | With depth control           |
| Random Forest       | Ensemble method              |
| AdaBoost            | Boosting technique           |
| XGBoost             | High-performance boosting    |
| SVM                 | With hyperparameter tuning   |

---

## 📈 Evaluation Metrics

- ✅ Confusion Matrix  
- ✅ Accuracy  
- ✅ Precision / Recall / F1-Score  
- ✅ Cross-validation  
- ✅ Comparison chart of all ML models

---

## 📷 Visualizations

- ✅ Attack category distributions  
- ✅ Label distributions (0 vs 1)  
- ✅ Feature correlation matrix heatmap  
- ✅ PCA 2D scatter plot  
- ✅ Confusion matrix heatmaps for models  
- ✅ Accuracy bar chart comparing all models  

---

## 🧪 How to Run

1. Ensure all required files are in the same directory.
2. Run the notebook file `UNSW_NB15___Cybersecurity_Threat_Detection.ipynb` using Jupyter Notebook or Google Colab.
3. Make sure necessary libraries such as `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`, and `imbalanced-learn` are installed.

---

## 👩‍💻 Authors

- **Mariam Ehab**
- **Omar Aymen**

> GitHub of Omar Aymen: `(https://github.com/omarayman142)`

---

## 🏁 Notes

- This project is a final evaluation for the Machine Learning track of the NTI Summer Internship 2025.
- All data cleaning, feature engineering, and model building steps are included in the notebook file.
