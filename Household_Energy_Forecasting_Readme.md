# Household Energy Consumption Time Series Forecasting

## 🚀 Project Overview
This project focuses on short-term forecasting of household energy usage using historical power consumption data.
The goal is to predict energy consumption patterns and compare the performance of multiple time series models.

## 📊 Objective
- Forecast short-term household energy usage based on historical patterns.
- Compare the predictive performance of different models: ARIMA, Prophet, XGBoost (optional).

## 🗂 Dataset
- **Dataset Name:** Household Power Consumption Dataset
- **Source:** [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/individual+household+electric+power+consumption)
- **Features:**
  - `Date` – Date of measurement
  - `Time` – Time of measurement
  - `Global_active_power` – Household active power (kW)
  - `Global_reactive_power`, `Voltage`, `Global_intensity`, `Sub_metering_1/2/3`

## 🛠 Instructions / Steps
1. **Data Preprocessing**
   - Load the dataset with `pandas`.
   - Combine `Date` and `Time` into a `datetime` column.
   - Convert `Global_active_power` to float and handle missing values.
   - Resample to daily frequency to reduce dataset size.
2. **Feature Engineering**
   - Create time-based features such as hour of day, weekday/weekend (optional for XGBoost).
3. **Modeling**
   - **ARIMA:** use `pmdarima.auto_arima` to find best `(p,d,q)` order, train on first 80%, forecast last 20%.
   - **Prophet:** fit Prophet on daily resampled data, forecast for test set length.
   - **XGBoost (optional):** use engineered time-based features for prediction.
4. **Evaluation**
   - Metrics: **MAE** and **RMSE**.
   - Compare ARIMA, Prophet, XGBoost (if implemented).
5. **Visualization**
   - Plot actual vs forecasted energy usage for each model.

## 📈 Skills Gained
- Time series forecasting
- Feature engineering for temporal data
- Model comparison and evaluation
- Temporal data visualization using Matplotlib
- Handling large datasets with pandas

## ⚡ Libraries Used
- `pandas`, `numpy`, `matplotlib`, `statsmodels`, `pmdarima`, `prophet`, `sklearn`, `xgboost` (optional)


## 📌 Notes
- The dataset is large (~2 million rows). Daily resampling is used to prevent memory and datetime errors.
- Prophet uses Stan under the hood; chain info messages are normal and can be suppressed.
- Optional XGBoost requires feature engineering for time-based inputs.


