
# Retail Sales Forecasting with Ensemble Learning
## This project builds an advanced time series forecasting system for retail sales using a combination of:

- Gradient Boosting Models (LightGBM, XGBoost)
- Statistical Time Series Model (Auto-ARIMA)
- Ensemble Learning (Residual Modeling + Weight Optimization)

The goal is to accurately predict weekly sales by leveraging store data, promotional features, and temporal patterns.

# Architecture

## Pipeline:
- Data Loading
- Data Merging
- Feature Engineering
- Model Training (LGBM, XGBoost)
- Residual Modeling (ARIMA)
- Ensemble + Optimization
  
## Tech Stack
- Python 
- Pandas, NumPy
- Scikit-learn
- LightGBM
- XGBoost
- pmdarima (Auto-ARIMA)
- Matplotlib

# Dataset Description
## File	Description
- train.csv:	Historical sales data
- test.csv:	Future dates for prediction
- features.csv:	Promotional & markdown data
- stores.csv:	Store metadata (type, size)

# Feature Engineering
## Extracted:
- Year, Month, Week, Day
- DayOfWeek, WeekOfYear
- Handled missing values (filled with 0)
- One-hot encoding for store types
- Converted holiday flags into numeric features

## Models Used
1. LightGBM:
Fast and efficient gradient boosting,
Handles large datasets well
2. XGBoost:
High-performance boosting algorithm,
Strong baseline comparison
3. Auto-ARIMA:
Captures time-based residual patterns,
Adds statistical learning on top of ML predictions
