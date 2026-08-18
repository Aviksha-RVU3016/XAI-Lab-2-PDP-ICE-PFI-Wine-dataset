# XAI-Lab-2-PDP-ICE-PFI-Wine-dataset
XAI Lab 2 – Explainable AI using PDP, ICE, and PFI on the Wine Quality Dataset

## Experiment Title

**Explainable AI Using Partial Dependence Plot (PDP), Individual Conditional Expectation (ICE), and Permutation Feature Importance (PFI)**
---
## Dataset
The experiment uses the **UCI Wine Quality Dataset** to build a machine learning model for predicting wine quality from its physicochemical properties.
---
## Objectives
The experiment applies three Explainable AI techniques:
- **Partial Dependence Plot (PDP)** – to understand the average effect of a feature on model predictions.
- **Individual Conditional Expectation (ICE)** – to understand how a feature affects predictions for individual samples.
- **Permutation Feature Importance (PFI)** – to identify the features that have the greatest impact on model performance.
---
## Machine Learning Model
A **Random Forest Regression** model is trained to predict wine quality.
The model is evaluated using:
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- R² Score

---

## XAI Techniques

### 1. Partial Dependence Plot (PDP)

PDP is used to study the average relationship between selected features and predicted wine quality.

Selected features:

- Alcohol
- Volatile Acidity
- Sulphates

### 2. Individual Conditional Expectation (ICE)

ICE plots are generated for the same three features using individual wine samples to examine how predictions vary across samples.

### 3. Permutation Feature Importance (PFI)

PFI is calculated for all input features by measuring the decrease in model performance after randomly permuting each feature.

---

## Results

The experiment demonstrates that **alcohol, sulphates, and volatile acidity** are among the most influential features according to the PFI analysis.

The PDP and ICE analyses further illustrate the relationships between these features and predicted wine quality.

Detailed results, plots, observations, and discussion are provided in the laboratory report.

---

## Files

| File | Description |
|---|---|
| `XAI_Lab_2_Wine_PDP_ICE_PFI.ipynb` | Complete Jupyter Notebook |
| `XAI_Lab_2_Report.docx` | Laboratory Report |
| `XAI_Lab_2_Report.pdf` | PDF version of the Laboratory Report |

---

## Conclusion

PDP, ICE, and PFI provide complementary explanations of the Random Forest model by describing feature effects, individual prediction behavior, and feature importance. Together, these techniques provide a better understanding of the model's behavior for wine quality prediction.
