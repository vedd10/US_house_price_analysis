# 🏡 House Price Analysis & Forecasting

This project analyzes and forecasts U.S. national home prices using publicly available economic indicators. It utilizes multiple regression and time series models including ARIMA and XGBoost to predict the Case-Shiller U.S. National Home Price Index.

---

## 📊 Data Sources

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

## 📈 Models Implemented

### 1. Regression Models (on Economic Features)

* Linear Regression
* Ridge Regression
* Lasso Regression
* ElasticNet
* Random Forest
* XGBoost ✅ (Best performing, RMSE \~0.15)

### 2. Time Series Model

* ARIMA model to forecast future Case-Shiller Index values.

---

## 🛠️ Feature Engineering

* Merged multiple CSV files on `observation_date`.
* Forward-filled missing values (`ffill`).
* No scaling used (optional: `StandardScaler` for linear models).

---

## 🧪 Evaluation Metrics

* RMSE (Root Mean Squared Error)
* R² Score

---

## 🔮 Forecasting Insights

* Used lag features with XGBoost to simulate time series prediction.
* ARIMA captured long-term trends with reasonable accuracy.

---

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first.

