# Assignment #7 - ARIMA Forecasting

## Dataset Overview

This assignment uses the **Retail Sales: Electronics Stores** dataset from the Federal Reserve Bank of St. Louis (FRED).

- **Series ID:** MRTSSM443142USN
- **Period:** January 2016 – December 2025
- **Frequency:** Monthly
- **Units:** Millions of Dollars
- **Seasonal Adjustment:** Not Seasonally Adjusted

## ARIMA Model

The `auto.arima()` function selected an **ARIMA(1,0,1)(0,1,1)[12]** model.

The assignment includes:

1. Time series exploration and stationarity testing.
2. ARIMA model selection and interpretation.
3. Residual diagnostics and the Ljung–Box test.
4. Five-month forecasts for January–May 2026.
5. Training and test set accuracy evaluation.

## Forecast Accuracy

The model was trained on January 2016–December 2024 and evaluated on January–December 2025.

| Metric | Test Set |
|---|---:|
| RMSE | 227.33 |
| MAE | 188.90 |
| MAPE | 3.17% |
| Theil's U | 0.2801 |

The ARIMA model outperformed ETS and Holt-Winters based on test RMSE, although Seasonal Naive achieved the lowest RMSE among the models compared.

## Files

- `Assignment 7 - ARIMA.Rmd` — R Markdown source code and analysis.
- `Assignment-7---ARIMA.html` — Rendered HTML report.
- `Retail Sales - Electronics Stores.csv` — Original dataset used in the analysis.

## Data Source

Federal Reserve Bank of St. Louis (FRED): [Retail Sales: Electronics Stores](https://fred.stlouisfed.org/series/MRTSSM443142USN)
