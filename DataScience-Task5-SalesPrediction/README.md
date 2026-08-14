
# Sales Prediction Using Python

## Project Overview

This project focuses on predicting product sales based on advertising expenditure across three media channels: TV, Radio, and Newspaper.

The project uses machine learning regression techniques to understand the relationship between advertising spending and sales and to build a model capable of predicting sales.

## Objective

The objective is to build and compare regression models that predict Sales using:

- TV advertising expenditure
- Radio advertising expenditure
- Newspaper advertising expenditure

## Dataset

The project uses the Advertising dataset containing 200 records.

### Features

- TV
- Radio
- Newspaper

### Target

- Sales

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Project Workflow

1. Data loading
2. Data understanding
3. Missing-value checking
4. Duplicate checking
5. Data cleaning
6. Exploratory Data Analysis
7. Pairplot analysis
8. Scatter plot analysis
9. Correlation heatmap
10. Train/test split
11. Linear Regression
12. Random Forest Regression
13. Model evaluation
14. Feature importance analysis
15. Residual analysis
16. Model comparison
17. Final conclusion

## Machine Learning Models

### Linear Regression

MAE: 1.461  
RMSE: 1.782  
R²: 0.899

### Random Forest Regressor

MAE: 0.620  
RMSE: 0.769  
R²: 0.981

## Model Comparison

Random Forest performed better than Linear Regression on all three evaluation metrics.

| Model | MAE | RMSE | R² |
|---|---:|---:|---:|
| Linear Regression | 1.461 | 1.782 | 0.899 |
| Random Forest | 0.620 | 0.769 | 0.981 |

Therefore, **Random Forest Regressor was selected as the best-performing model.**

## Feature Importance

| Feature | Importance |
|---|---:|
| TV | 0.624810 |
| Radio | 0.362214 |
| Newspaper | 0.012976 |

### Key Finding

**TV advertising has the highest impact on sales**, followed by Radio. Newspaper has the lowest importance according to the Random Forest model.

## Residual Analysis

Residuals were calculated as:

`Residual = Actual Sales - Predicted Sales`

The residual plot was used to check whether the model's errors were randomly distributed around the zero line.

## Conclusion

This project successfully developed a machine learning solution for sales prediction using advertising expenditure.

Two regression models were evaluated. Random Forest Regressor achieved the best performance with an R² score of 0.981, MAE of 0.620, and RMSE of 0.769.

Feature importance analysis showed that TV advertising was the most influential channel in predicting sales.
