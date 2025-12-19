## Overview
A comparative analysis of Ridge, LASSO, and Best Subset Selection regression models to predict median home values. The goal was to identify the optimal regularization technique for preventing overfitting on a classic dataset.

## Methods
- **Models:** Ridge Regression (L2), LASSO (L1), Best Subset Selection
- **Validation:** 10-fold cross-validation
- **Evaluation Metrics:** Mean Squared Error (MSE), R-squared
- **Tools:** R (ggplot2, glmnet, leaps packages)

## Key Results
- The **LASSO model** achieved the lowest test MSE (X.XX) and identified 7 key predictive features.
- Ridge regression provided more stable coefficient estimates than OLS but retained all 13 predictors.
- Coefficient shrinkage paths visualized the bias-variance tradeoff clearly.
