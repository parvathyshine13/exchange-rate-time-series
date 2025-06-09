# 📈 Forecasting Exchange Rates using Time Series Analysis  

## 🗂️ Data Preparation and Exploration
- Visualized the raw time series to understand overall trend, stationarity, and potential seasonality.
- Identified and interpolated missing values to ensure data continuity.

## 🌀 ARIMA Model Implementation
- Used ACF and PACF plots to determine the best parameters (p, d, q) for the ARIMA model.
- Fit the ARIMA model on the cleaned time series data.
- Conducted residual analysis to verify that no significant patterns remained, confirming a good fit.
- Forecasted future exchange rates and plotted them alongside actual historical data for comparison.

## 📉 Exponential Smoothing Approach
- Chose Holt’s Linear Trend model based on the presence of a trend but no clear seasonality.
- Tuned smoothing parameters using grid search and AIC to find the most optimal configuration.
- Forecasted future values using the fitted model and visualized results against actual data points.

## 📊 Evaluation and Model Comparison
- Calculated MAE, RMSE, and MAPE to compare the ARIMA and Exponential Smoothing forecasts.
- Found ARIMA slightly outperformed in terms of lower RMSE and better fit to short-term fluctuations.
- Noted Holt's method offered smoother long-term trends, useful for less volatile forecasts.

## 🧰 Tools & Libraries Used
- **Python** for scripting and model building
- **Pandas** for data loading and preprocessing
- **Matplotlib / Seaborn** for visualization
- **Statsmodels** for ARIMA model and statistical tools (ACF, PACF)
- **Scikit-learn** for error metric evaluation
- **Statsmodels.tsa.holtwinters** for Exponential Smoothing
