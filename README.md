# Healthcare Premium Prediction – Statistical Computing and Machine Learning Project

This project analyzes a large, anonymized insurance dataset from Kaggle (1.2 million entries) to build predictive models for healthcare premium pricing using both parametric and non-parametric methods.

---

## Project Summary

- **Objective:** Predict insurance premium amounts using demographic, behavioral, and financial variables.
- **Data:** 1.2M rows, 20+ features including income, health score, credit score, feedback, location, and lifestyle.
- **Tools:** R, `ggplot2`, `MASS`, `FNN`, `caret`, `dplyr`

---

## Jump In Improvement Within Our Methods & Results

| Model | Description | R² | RMSE |
|-------|-------------|----|------|
| Linear Regression | Stepwise AIC-selected model | 0.003 | ~$867.90 |
| **KNN (Log Transformed)** | Final model (log + scaled features) | **0.63** | **$528.73** |

- Stepwise regression revealed key interaction effects between claims, credit, income, and feedback.
- KNN was more flexible and outperformed linear approaches significantly.
- Final model validated with 5-fold cross-validation.

---


##  Key Learnings

- Linear models are often inadequate for skewed real-world data with complex interactions.
- Feature scaling and transformations are critical for KNN performance.
- Cross-validation ensures that model results generalize across samples.
- This projects highlights the need for non-parametric models in actuarial sciences
---
