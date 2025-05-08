# 🧠 Predicting Breast Cancer Risks with Explainable AI

## 📌 Project Overview

This project applies advanced machine learning models and **Explainable AI (XAI)** techniques to predict whether breast cancer tumors are benign or malignant. The goal is to build not only a highly accurate model, but also one that offers **transparency and interpretability** — critical for clinical decision-making.

## 🎯 Objectives

- Develop predictive models for breast cancer classification.
- Implement a **stacking ensemble** to boost performance.
- Use **SHAP**, **LIME**, and **PDP** to explain model predictions.
- Deploy insights to support early detection and medical decisions.


| Feature | Description |
|--------|-------------|
| 🎯 **Goal** | Predict breast cancer malignancy from diagnostic data |
| 🧪 **Dataset** | [Wisconsin Diagnostic Breast Cancer (WDBC)](https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29) |
| 🛠 **Techniques** | ML Models (SVM, RF, MLP, XGBoost, CatBoost), Ensemble Stacking |
| 🔍 **Explainability** | SHAP, LIME, Partial Dependence Plots (PDP) |
| 🧠 **Framework** | CRISP-DM |
| 📊 **Evaluation** | Accuracy, Sensitivity, Specificity, Precision, F1-score, ROC-AUC |
| 📈 **Top Accuracy** | 96.74% with stacking classifier (AUC = 0.99) |
---


## 🔧 Tools & Technologies

| Tool | Purpose |
|------|---------|
| `Python` | Core programming |
| `Pandas`, `NumPy`, `Matplotlib`, `Seaborn` | EDA and preprocessing |
| `Scikit-learn`, `XGBoost`, `CatBoost` | Model development |
| `SHAP`, `LIME`, `PDPbox` | Explainable AI |
| `IsolationForest` | Outlier removal |
| `StandardScaler`, `RFE` | Feature scaling and selection |


---

## 🔬 Methodology Overview

Following the **CRISP-DM** framework:

1. **Business Understanding** – Improve early breast cancer detection with interpretable AI.
2. **Data Understanding** – WDBC dataset; 569 samples with 32 features.
3. **Data Preparation** – Feature selection (RFE), outlier handling, scaling, class balancing (oversampling).
4. **Modeling** – Built SVM, RF, MLP, XGBoost, CatBoost, and a stacked ensemble model.
5. **Evaluation** – Used metrics like accuracy, F1-score, ROC-AUC.
6. **Interpretation** – Applied SHAP, LIME, PDP for insight into predictions.

---

## 📈 Model Performance Summary

| Model | Accuracy | AUC | Notes |
|-------|----------|-----|-------|
| SVM | 93.95% | ~0.96 | Solid linear boundary |
| Random Forest | 95.00% | ~0.97 | Robust tree ensemble |
| MLP | 95.00% | ~0.96 | Captures nonlinearities |
| XGBoost | 96.27% | ~0.98 | Best individual model |
| CatBoost | 96.27% | ~0.98 | Handles categorical data |
| **Stacking Classifier** | **96.74%** | **0.99** | Top performer (ensemble) |

---

## 🧠 Explainable AI (XAI) Results

| Technique | Highlights |
|----------|------------|
| `SHAP` | Identified top global features like `perimeter_worst`, `area_worst` |
| `LIME` | Explained individual predictions (e.g., why a tumor was classified malignant) |
| `PDP` | Showed how features like `radius_mean` influence model decisions |


## 📊 Results

- **Highest Accuracy**: Achieved using stacked model
- **Top Features**: Identified by SHAP values
- **Clinical Transparency**: Enhanced via SHAP/LIME visualizations
