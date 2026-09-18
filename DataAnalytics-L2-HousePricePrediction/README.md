

# House Price Prediction using Linear Regression

## Project Overview

This project focuses on predicting house prices using Machine Learning techniques. Housing dataset is used to analyze different property features and build regression models for predicting `SalePrice`.

The project covers the complete workflow from data exploration and preprocessing to model training, evaluation, and interpretation.

## Objective

The main objective is to build and evaluate a Linear Regression model for predicting house prices based on available property-related features.

## Dataset

The project uses the Housing dataset from the Kaggle House Prices competition.

- Dataset file: `train.csv`
- Target variable: `SalePrice`
- Number of records: 1460
- Original number of columns: 81

## Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Workflow

1. Load the dataset
2. Exploratory Data Analysis
3. Check missing values
4. Descriptive statistics
5. Analyze `SalePrice` distribution
6. Correlation analysis
7. Feature selection discussion
8. Handle missing values
9. One-Hot Encoding
10. Train-Test Split (80:20)
11. Train Linear Regression model
12. Predict house prices
13. Evaluate the model using MSE, RMSE, and R²
14. Analyze Actual vs Predicted prices
15. Perform residual analysis
16. Analyze model coefficients
17. Implement Ridge Regression
18. Implement Lasso Regression
19. Compare model performance

## Model Performance

| Model | RMSE | R² Score |

| Linear Regression | 31,080.81 | 0.8741 |
| Ridge Regression | 34,372.94 | 0.8460 |
| Lasso Regression | 43,911.84 | 0.7486 |

## Key Learning Outcomes

- Understanding and performing Exploratory Data Analysis
- Handling missing values
- Converting categorical variables using One-Hot Encoding
- Splitting data into training and testing sets
- Building regression models using Scikit-learn
- Evaluating regression models using MSE, RMSE, and R²
- Visualizing prediction errors and residuals
- Understanding regression coefficients
- Comparing regularized regression models

## Files

- `SnehaChorage_Task2.ipynb` – Complete Jupyter Notebook containing the analysis and machine learning implementation.
- `train.csv` – Dataset used for training and evaluation.


This project provided an end-to-end understanding of house price prediction using regression techniques. Linear Regression, Ridge Regression, and Lasso Regression were implemented and evaluated using standard regression metrics.
