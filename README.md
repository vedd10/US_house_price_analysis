# US_House_Price_Analysis
This repository contains a machine learning model to analyze and forecast U.S. home prices using the S&amp;P Case-Shiller Home Price Index (CSUSHPISA) along with various macroeconomic factors. The project involves data preprocessing, feature engineering, and model evaluation using techniques like Linear Regression, ARIMA, Random Forest, and XGBoost.

# Home Price Modeling

This repository contains a data science project aimed at forecasting U.S. home prices using the S&P Case-Shiller Home Price Index (CSUSHPISA) and key macroeconomic indicators. The goal is to understand how macroeconomic factors have influenced home prices over the last 20 years, using various machine learning models.

## Table of Contents

- [Project Overview]
- [Data Description]
- [Methodology]
- [Installation]
- [Modeling Techniques]
- [Results]
- [Contributors]

## Project Overview

This project aims to build predictive models to forecast home prices in the United States. By using features like inflation rates, unemployment rates, GDP growth, and mortgage rates, we explore their relationship with the home price index.

### Key Highlights:
- Data preprocessing using missing value handling and feature engineering.
- Multiple models used, including Linear Regression, ARIMA, Random Forest, and XGBoost.
- Time-series and non-time-series forecasting techniques.
- Model evaluation with R-squared (R²), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

## Data Description

The dataset used in this project consists of historical home price indices (S&P Case-Shiller Home Price Index) along with other macroeconomic indicators like GDP, inflation, and unemployment rates.

- **Source**: [FRED - Federal Reserve Economic Data](https://fred.stlouisfed.org/)
- **Data Fields**:
    - `observation_date`: Date of the observation
    - `CSUSHPISA`: Case-Shiller U.S. National Home Price Index (Target variable)
    - Additional macroeconomic features like GDP, unemployment rate, inflation rate, etc.

## Methodology

The project follows the below steps:

1. **Data Preprocessing**:
   - Cleaning and merging data from multiple CSV files.
   - Handling missing values using forward fill.
   - Feature engineering: Lag features for home price indices.

2. **Modeling**:
   - **Linear Regression**: Used for simple linear relationships between features and target.
   - **ARIMA**: Time-series model for predicting future values based on past observations.
   - **Random Forest**: A non-linear model to capture complex interactions between features.
   - **XGBoost**: Gradient boosting technique used for regression tasks.

3. **Evaluation**:
   - The models are evaluated using R-squared (R²), Mean Absolute Error (MAE), and Root Mean Squared Error (RMSE).

## Installation

Clone the repository to your local machine or Google Colab:

```bash
git clone https://github.com/your-username/home-price-modeling.git
cd home-price-modeling
