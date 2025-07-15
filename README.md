

# 🧬 Logistic Regression on Breast Cancer Dataset

This project involves applying **Logistic Regression** to classify malignant and benign tumors using the **Breast Cancer Wisconsin Dataset**. The goal is to build an accurate binary classification model, evaluate its performance using key metrics, and tune decision thresholds to understand model behavior.

---

## 📌 Project Highlights

### ✅ Dataset Overview

* **Entries:** 569
* **Features:** 30 numeric features describing cell nuclei properties
* **Target Variable:** `diagnosis` — Malignant (M) or Benign (B)

---

## 🔍 Steps Performed

### 1. **Data Loading & Cleaning**

* Removed unnecessary columns (`id`, unnamed columns)
* Converted target `diagnosis` to binary: `M=1`, `B=0`
* Checked for missing/null values

### 2. **Data Splitting & Standardization**

* Split data into `train` and `test` sets (80:20 ratio)
* Standardized features using `StandardScaler` to ensure uniform scaling

### 3. **Model Training**

* Implemented **Logistic Regression** using `sklearn`
* Trained the model on scaled training data
* Predicted outcomes on test data

---

## 📈 Model Evaluation

* ✅ **Confusion Matrix:**

  ```
  [[70  1]
   [ 2 41]]
  ```

* ✅ **Classification Report:**

  * Precision: 97% (Benign), 98% (Malignant)
  * Recall: 98% (Benign), 95% (Malignant)
  * F1 Score: 97%+

* ✅ **ROC-AUC Score:** `0.997` — indicates excellent model discrimination

* ✅ **ROC Curve:** Plotted to visualize performance at different thresholds

---

## 🔧 Threshold Tuning

* Evaluated model performance using custom thresholds (0.4, 0.5, 0.6)
* Observed trade-offs between **precision**, **recall**, and **F1-score**
* Used sigmoid-based predicted probabilities for adjusting cutoffs

---

## 🧠 Concepts Applied

* Logistic Regression
* Sigmoid Function
* Confusion Matrix, ROC Curve, AUC
* Precision, Recall, F1 Score
* Threshold Tuning
* Standardization

---

## 📁 Tech Stack

* **Python**
* **Pandas, NumPy**
* **Scikit-learn**
* **Matplotlib, Seaborn**

---

## 📊 Results Summary

| Threshold | Precision | Recall | F1 Score |
| --------- | --------- | ------ | -------- |
| 0.4       | 0.9767    | 0.9767 | 0.9767   |
| 0.5       | 0.9762    | 0.9534 | 0.9647   |
| 0.6       | 1.0000    | 0.9534 | 0.9761   |

---

## 🔗 Notebook Access

You can view the full notebook here:
👉 [Open in Colab](https://colab.research.google.com/drive/1AaGd7-94wrjDtYF32wFA8jiuEUrKA3DZ)


