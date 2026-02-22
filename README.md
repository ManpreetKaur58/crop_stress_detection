# Early Crop Stress Detection Using Multispectral Data

## Project Overview
This project focuses on detecting early crop stress using multispectral vegetation indices and machine learning models. The goal is to identify stressed areas before visible symptoms appear.

---

## Dataset
The dataset includes vegetation indices and supporting spatial features:

- NDVI (mean, min, max, std)
- GNDVI
- EVI
- SAVI
- Red Edge 1 & 2
- NIR Reflectance
- Moisture Index
- Canopy Density
- Grid X, Grid Y

Target variable:
- Crop Health (Healthy / Stressed)

---

## Exploratory Data Analysis
- Feature distribution histograms
- Correlation heatmap
- Feature subset analysis (early stress vs overall condition)
- Pair plots

---

## Models Used

### 1️ Logistic Regression
- Stratified K-Fold Cross Validation
- Threshold tuning
- ROC Curve
- Confusion Matrix
- Stress Heat Map

### 2️ Random Forest
- Stratified K-Fold
- GridSearchCV hyperparameter tuning
- Feature Importance
- ROC Curve
- Stress Heat Map

---

## Model Performance Summary

| Metric        | Logistic Regression | Random Forest |
|--------------|--------------------|---------------|
| Accuracy     | 0.842              | 0.862         |
| Precision    | 0.725              | 0.758         |
| Recall       | 0.881              | 0.893         |
| ROC-AUC      | 0.935              | 0.923         |
| F1 Score     | 0.796              | 0.820         |

---

## Stress Heat Maps
Both models generate field-level stress probability maps using grid coordinates.

These maps help prioritize inspection zones.

---

## Technologies Used
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
- imbalanced-learn (SMOTE)

---

## 🚀 How to Run

1. Clone the repository
2. Install requirements:
