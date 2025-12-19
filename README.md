# Boston Housing Price Prediction: Regularization Methods

## Methods
- **Dataset:** Boston Housing (506 observations, 13 predictors)
- **Models:** Best Subset Selection (BIC), LASSO (L1), Ridge Regression (L2)
- **Validation:** 70/30 train-test split
- **Tools:** R (glmnet, leaps, hdi)

## Results
| Method | Validation MSE | Validation R² |
|--------|---------------|---------------|
| Ridge Regression | 27.223 | 0.596 |
| LASSO | 27.320 | 0.595 |
| Best Subset Selection | 28.801 | 0.573 |

**Findings:**
- Ridge had the best prediction accuracy (lowest MSE)
- LASSO performed almost as well with only 9 predictors
- Best Subset showed the most overfitting
- Key predictors: room count, neighborhood status, school quality

## Files
- `stat435_Project_Berlage_Pascal.Rmd` - Complete R Markdown analysis
- `boston_housing_report.pdf` - Analysis as PDF
- `README.md` - This file
