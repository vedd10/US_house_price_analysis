# House Price Analysis & Forecasting

This project analyzes and forecasts U.S. national home prices using publicly available economic indicators. It utilizes multiple regression and time series models including ARIMA and XGBoost to predict the Case-Shiller U.S. National Home Price Index.

---

## Data Sources

Economic indicators downloaded from FRED (Federal Reserve Economic Data):

* CPIAUCSL — Consumer Price Index
* CSUSHPISA — Case-Shiller Home Price Index (target variable)
* CUUR0000SEHA — Rent Index
* FEDFUNDS — Federal Funds Rate
* GDP, GDPC1 — Gross Domestic Product (nominal and real)
* POPTHM — Population
* MEHOINUSA672N — Median Household Income
* UNRATE — Unemployment Rate
* MORTGAGE30US — Mortgage Rates
* RHORUSQ156N — Homeownership Rate
* HOUST, PERMIT — Housing Starts & Permits

---


## Models Used

| Model              | Description                                                                 |
|-------------------|-----------------------------------------------------------------------------|
| Linear Regression  | Baseline model. Interpretable and performs well with standardized features. |
| Random Forest      | Handles nonlinearities and interactions, provides feature importance.       |
| XGBoost            | Boosted tree model, robust and highly accurate for tabular data.            |
| ARIMA              | Time series forecasting model, good at capturing temporal patterns.         |

---

## Results

- **Best Model**: Linear Regression (based on R², MAE, RMSE).
- **Top Influencing Features**:
  - Lagged values of the home price index
  - Mortgage rates
  - Consumer price index (CPI)
  - Unemployment rate

---

## 📈 Visualizations

- Home price index trend over time
- Actual vs Predicted plots
- Feature importance charts
- Correlation matrix heatmap

---

## 🛠️ Requirements

- Python 3.7+
- Google Colab (for running notebook)
- Libraries:
  - `pandas`, `numpy`, `matplotlib`, `seaborn`
  - `scikit-learn`, `xgboost`, `statsmodels`

---

## 🚀 How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/home-price-prediction.git
   cd home-price-prediction


