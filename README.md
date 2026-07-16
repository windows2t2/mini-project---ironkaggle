# IronKaggle — King County House Price Prediction

A machine learning project predicting house sale prices in King County, Washington (May 2014 – May 2015). Part of the Ironhack Data Analytics Bootcamp.

## Overview

The goal is to explore, clean, and model a dataset of home sales to find which features best predict price. The project covers the full ML workflow: loading data, EDA, training regression models, evaluation, and selecting the best model.

## Data

**Source:** [Kaggle — King County Houses AA](https://www.kaggle.com/datasets/minasameh55/king-country-houses-aa)

The dataset (`king_county_houses_aa.csv`) has 21 columns including bedrooms, bathrooms, sqft_living, sqft_lot, floors, waterfront, view, condition, grade, yr_built, yr_renovated, zipcode, lat, long, and price (the target).

## Approach

1. Load and explore the data
2. Clean and parse dates
3. Train-test split (80/20)
4. Correlation analysis
5. Encode and standardize features
6. Train 8 regression models
7. Evaluate with R², MAE, and RMSE
8. Select the best model

## Models

Linear Regression, Lasso, Ridge, K-Nearest Neighbors, Decision Tree, Random Forest, Gradient Boosting, AdaBoost

## How to Run

```bash
git clone https://github.com/windows2t2/mini-project---ironkaggle.git
cd mini-project---ironkaggle
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
jupyter notebook mycode.ipynb
```

## Tech Stack

Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, Jupyter Notebook

## Future Work

- Outlier handling and feature engineering
- Hyperparameter tuning (GridSearchCV)
- Try XGBoost, LightGBM, or CatBoost
- Cross-validation for more robust results
