
# Ames Housing Price Prediction

**IT3091 Machine Learning Group Project — Group 2026-DS-18**

## Project Overview

This project focuses on predicting residential house prices using the Ames Housing dataset. We explored the data, performed preprocessing and feature engineering, developed multiple regression models, and compared their predictive performance.

## Machine Learning Models

We developed and evaluated four regression models:

- Linear Regression
- Random Forest
- Gradient Boosting
- XGBoost

## Project Workflow

1. Problem framing and understanding the dataset
2. Exploratory Data Analysis (EDA)
3. Data cleaning and preprocessing
4. Feature engineering
5. Model development and training
6. Model validation and comparison
7. Results analysis and recommendations

The target variable, SalePrice, was log-transformed using log1p during model development.

## Model Validation Results

The following results are from the nested cross-validation comparison:

| Model | RMSE | MAE | R² |
|---|---:|---:|---:|
| Gradient Boosting | 0.1297 | 0.0853 | 0.8897 |
| XGBoost | 0.1311 | 0.0852 | 0.8872 |

Gradient Boosting was selected based on its slightly lower RMSE. The difference between the two models was small and should not be interpreted as conclusive statistical superiority.

**Note:** These metrics are based on the log-transformed target, not house prices in dollars.

## Dataset

The project uses the Ames Housing dataset from the Kaggle House Prices: Advanced Regression Techniques competition.

The raw training and test CSV files are not included in this repository. Download them from Kaggle and place them in the Dataset folder when running the notebooks.

Dataset source:
https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data

## Repository Structure

- `Dataset/` — Dataset documentation and data dictionary
- `Documentation/` — Problem framing, workflow and decision logs
- `Notebooks/` — Model development, preprocessing and validation notebooks
- `Results_and_evidence/` — EDA evidence, model graphs and results
- `Final_Group_Report/` — Group project report, subject to team approval
- `YouTube_Demo_Link.txt.md` — Project demonstration video link

## Interactive Application

A Streamlit application was created to demonstrate the house price prediction workflow.

[Open the Ames Housing Prediction Application](https://house-price-app-mwqvkykedd69l42rnnfbvv.streamlit.app/)

## Technologies Used

- Python
- Pandas and NumPy
- Scikit-learn
- XGBoost
- Matplotlib and Seaborn
- Jupyter Notebook
- Streamlit

## Academic Project

This project was completed as part of the IT3091 Machine Learning module by Group 2026-DS-18.

The application is an academic demonstration and its predictions should not be treated as official property valuations.
