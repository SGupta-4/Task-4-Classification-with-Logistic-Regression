# Logistic Regression Classifier - Breast Cancer Detection

## Objective
Build a binary classifier using Logistic Regression to predict whether a tumor is **malignant (M)** or **benign (B)** using the **Breast Cancer Wisconsin dataset**.

---

## Dataset
The dataset contains medical features computed from digitized images of breast masses.  
Columns include tumor characteristics such as **radius_mean, texture_mean, perimeter_mean, area_mean, smoothness_mean**, etc.  

Key details:
- **Target column:** `diagnosis`  
  - M = Malignant (1)  
  - B = Benign (0)  
- Dropped columns: `id`, `Unnamed: 32`  

---

## Steps
1. **Data Preprocessing**
   - Dropped irrelevant columns.
   - Converted target labels (`M`, `B`) into binary values (1, 0).
   - Standardized features using `StandardScaler`.

2. **Train-Test Split**
   - Split dataset into **80% training** and **20% testing**.
   - Stratified sampling to maintain class balance.

3. **Model Training**
   - Trained a **Logistic Regression** model with scikit-learn.

4. **Evaluation**
   - **Confusion Matrix**
   - **Classification Report** (Precision, Recall, F1-score)
   - **ROC-AUC Score**
   - **ROC Curve** plot

5. **Threshold Tuning**
   - Used predicted probabilities and ROC curve to analyze different thresholds.

---

## Results
- Logistic Regression achieved high performance on this dataset.
- ROC-AUC Score indicates good separation between malignant and benign cases.
- Confusion matrix and metrics highlight strong precision and recall.

---

## Tools Used
- **Python**
- **Pandas**
- **Scikit-learn**
- **Matplotlib**

---
