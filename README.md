# Stock-Market-Forecasting-using-AutoARIMA-2025-2026-
This project applies advanced time-series forecasting techniques to predict stock indices—NIFTY 50 and S&P 500—using Python and the AutoARIMA model. The forecasts span from 2015 to early 2025 with the goal of extending predictions for the next 5–6 months. This notebook is designed for financial research, market insight generation, and academic exploration.

Project Objectives
📌 Forecast future values of NIFTY 50 and S&P 500 indices using AutoARIMA.

📌 Evaluate stationarity and seasonal behavior in historical data.

📌 Visualize time series trends, residuals, and model fit.

📌 Deploy a reproducible workflow for financial time series forecasting.

Data Collection & Preprocessing- 
- Data Source: Yahoo Finance

- Ticker Symbols:

NIFTY 50: ^NSEI

S&P 500: ^GSPC

- Time Frame: March 2015 – March 2025


Preprocessing Steps:

1. Download historical data using yfinance.

2. Select relevant columns (Date, Close, etc.).

3. Handle missing values and log-transform closing prices for stationarity.

4. Perform seasonal decomposition and stationarity testing.

 Model: AutoARIMA
 
- Utilizes pmdarima’s auto_arima() to automate model selection.

- Log-transformed data improves stability and removes exponential growth trends.

- Key Evaluation Metrics:

AIC (Akaike Information Criterion)

RMSE on test set

Residual diagnostics


Forecast Output
Models trained separately for:

- df_nifty_log → NIFTY 50 forecast

- df_sp500_log → S&P 500 forecast

Forecast plots include:

1. Actual vs Forecasted values

2. Confidence Intervals

3. Residual distribution

Dependencies
1. pandas

2. numpy

3. matplotlib

4. seaborn

5. statsmodels

6. pmdarima

7. yfinance

8. scikit-learn

 Visuals Included
- Time Series Line Plots

- Seasonal Decomposition

- ADF & Rolling Statistics

Forecast vs Actual Line Graphs

Requirements - 
pandas
numpy
matplotlib
seaborn
statsmodels
pmdarima
yfinance
scikit-learn

Result - 
- Both indices show clear long-term trends with short-term fluctuations.

- Log transformation + differencing helped achieve stationarity.

- AutoARIMA is robust for univariate financial forecasting when exogenous variables are not included.














