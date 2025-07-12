# 💡 Healthcare Premium Prediction – Statistical Computing Project

This project analyzes a large, anonymized insurance dataset from Kaggle (1.2 million entries) to build predictive models for healthcare premium pricing using both parametric and non-parametric methods.

---

## 📊 Project Summary

- **Objective:** Predict insurance premium amounts using demographic, behavioral, and financial variables.
- **Data:** 1.2M rows, 20+ features including income, health score, credit score, feedback, location, and lifestyle.
- **Tools:** R, `ggplot2`, `MASS`, `FNN`, `caret`, `dplyr`

---

## 🔬 Methods & Results

| Model | Description | R² | RMSE |
|-------|-------------|----|------|
| Linear Regression | Stepwise AIC-selected model | 0.009 | ~$867 |
| Box-Cox Regression | Transformed response | 0.0176 | ~$700 |
| **KNN (Log Transformed)** | Final model (log + scaled features) | **0.63** | **$528.73** |

- Stepwise regression revealed key interaction effects between claims, credit, income, and feedback.
- KNN was more flexible and outperformed linear approaches significantly.
- Final model validated with 5-fold cross-validation.

---

## 📁 Files

| File | Description |
|------|-------------|
| `Full_Report.pdf` | Complete write-up with diagnostics, plots, and conclusions |
| `sta160_code.Rmd` | Full annotated R code used in the analysis |
| `outputs/` | Visuals like correlation plots and prediction results |

---

## 📌 Key Learnings

- Linear models are often inadequate for skewed real-world data with complex interactions.
- Feature scaling and transformations are critical for KNN performance.
- Cross-validation ensures that model results generalize across samples.

---
