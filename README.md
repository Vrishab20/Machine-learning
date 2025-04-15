# Explainable AI (XAI) - Assignment 2  
**Course:** CSI5155 - Fall 2024  
**Author:** Vrishab Davey  
**Student ID:** 300438343  

## Overview  
This project explores the interpretability of machine learning models using SHAP (SHapley Additive exPlanations) on two datasets: Chocolate and Mushroom. Models analyzed include Random Forests and Decision Trees. The goal was to understand **why models make certain predictions**, **when they succeed or fail**, and how **to improve future model performance**.

---

## Datasets  
- **Chocolate Dataset**  
- **Mushroom Dataset**

---

## Best & Worst Models  

| Dataset   | Best Model (Accuracy)     | Worst Model (Accuracy)    |
|-----------|---------------------------|----------------------------|
| Chocolate | Random Forest – 72.94%    | Decision Tree – 72.41%    |
| Mushroom  | Random Forest – 73.79%    | Decision Tree – 68.33%    |

---

## SHAP-Based Insights  

### Feature Importance  
- **Chocolate Dataset:**  
  - Influential: `Ethnicity`, `Ascore`, `Cscore`, `Escore`  
  - Random Forest captured more complex patterns due to deeper trees and more estimators.

- **Mushroom Dataset:**  
  - Influential: `Country`, `Age`, `SS`  
  - Decision Tree underperformed due to shallow structure and inability to model complex interactions.

### Why Certain Predictions Weren’t Made  
- Features like `Gender` and `Country` had negligible SHAP impact in some models, explaining their limited role in predictions.

### Model Trust & Improvements  
- **Random Forests:** More reliable due to their capacity to model intricate feature interactions. Further tuning (e.g., increasing estimators, adjusting depth) can boost performance.  
- **Decision Trees:** Easier to interpret but less reliable. Accuracy may improve with deeper trees and feature engineering.

---

## Conclusion  
SHAP proved valuable in demystifying model decisions and highlighting paths for refinement. While Random Forests outperformed Decision Trees in both datasets, the latter's interpretability offers useful trade-offs for simpler domains.
