# Machine Learning Project - GDP Prediction

This project applies a **Multi-Layer Perceptron (MLP) Regressor** to predict GDP based on multiple economic indicators.  This project was done for Machine Learning course.
It uses **scikit-learn** with a pipeline, hyperparameter tuning, and visualization of results.

## Project Overview

- **Data Source**: `factbookv2.csv`
- **Goal**: Predict GDP from selected economic indicators
- **Techniques Used**:
  - Data cleaning and preprocessing
  - Feature scaling with `StandardScaler`
  - Train-test split (80/20)
  - Hyperparameter tuning using `GridSearchCV`
  - Evaluation with **MSE** and **R²**
  - Visualization of Actual vs Predicted values

## Features Used

The following economic indicators are used as features:
- GDP (target)
- Exports
- Imports
- Industrial production growth rate
- Investment
- Unemployment rate

## Workflow

1. **Data Cleaning**  
   - Remove `$` and `,` symbols from numeric values  
   - Handle missing values  

2. **Preprocessing**  
   - Standardize features with `StandardScaler`  
   - Split into `X` (features) and `y` (GDP)  

3. **Modeling**  
   - `MLPRegressor` wrapped in a pipeline  
   - Hyperparameter tuning with **GridSearchCV**  
   - Cross-validation with `KFold (n_splits=5)`  

4. **Evaluation**  
   - Compute **MSE** and **R²** on training and test sets  
   - Scatter plots comparing Actual vs Predicted values  

