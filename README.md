# Boston Housing Price Prediction: Regularization Methods

## Project Description
This project compares three regression methods—Best Subset Selection, LASSO, and Ridge Regression—to predict median home values using the Boston Housing dataset. The goal was to see which method gives the best prediction accuracy while handling correlated predictors.

## Methods
- **Dataset:** Boston Housing (506 observations, 13 predictors)
- **Models compared:** Best Subset Selection (BIC), LASSO (L1), Ridge Regression (L2)
- **Validation:** 70/30 train-test split
- **Tools:** R (glmnet, leaps, hdi packages)

## Results Summary
| Method | Validation MSE | Validation R² |
|--------|---------------|---------------|
| Ridge Regression | 27.223 | 0.596 |
| LASSO | 27.320 | 0.595 |
| Best Subset Selection | 28.801 | 0.573 |

**Key findings:**
- Ridge Regression had the best prediction accuracy (lowest MSE)
- LASSO performed almost as well as Ridge while selecting only 9 significant predictors
- Best Subset Selection showed the most overfitting (highest MSE)
- Important predictors in all models: room count (`rm`), neighborhood status (`lstat`), and school quality (`ptratio`)

## How to Run
1. Clone this repository
2. Open `boston_analysis.R` in R or RStudio
3. Install required packages: `install.packages(c("glmnet", "leaps", "hdi", "MASS"))`
4. Run the script to reproduce the analysis

## Files
- `boston_analysis.R` - Main analysis script
- `README.md` - This file
