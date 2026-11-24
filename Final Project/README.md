
# Final Project - Forecasting U.S. Electronics Store Retail Sales

## Project Overview

The objective of this project is to forecast monthly U.S. electronics store retail sales for January–May 2026 using historical time series data. The analysis compares four forecasting models to determine which provides the most accurate predictions.

This topic was selected because of my experience working in electronics retail and my interest in understanding seasonal sales patterns. Accurate retail sales forecasts can support inventory management, staffing, budgeting, and promotional planning.

## Dataset Overview

- **Dataset:** Retail Sales: Electronics Stores
- **Source:** U.S. Census Bureau via FRED
- **Series ID:** MRTSSM443142USN
- **Time Period:** January 2016 – December 2025
- **Frequency:** Monthly
- **Number of Observations:** 120
- **Units:** Millions of U.S. Dollars
- **Seasonal Adjustment:** Not Seasonally Adjusted

## Forecasting Methodology

Four forecasting models were evaluated:

- Seasonal Naive
- Seasonal ARIMA(1,0,1)(0,1,1)[12]
- Exponential Smoothing (ETS)
- Holt-Winters Additive

The models were trained using data from January 2016 through December 2024 and evaluated against actual sales from January through December 2025.

Root Mean Squared Error (RMSE) was used as the primary model selection metric, with MAE and MAPE serving as additional accuracy measures. Residual diagnostics and Ljung–Box tests were also performed to evaluate model adequacy.

## Model Comparison

| Model | Test RMSE | Test MAE | Test MAPE |
|---|---:|---:|---:|
| **Seasonal Naive** | **196.07** | **154.58** | **2.71%** |
| ARIMA | 227.33 | 188.90 | 3.17% |
| Holt-Winters | 258.59 | 194.84 | 3.41% |
| ETS | 261.66 | 198.37 | 3.47% |

RMSE and MAE are measured in millions of dollars.

## Final Model Selection

Seasonal Naive was selected as the recommended forecasting model because it achieved the lowest out-of-sample RMSE, MAE, and MAPE among the four models evaluated.

Although residual diagnostics revealed significant remaining autocorrelation, Seasonal Naive demonstrated the strongest forecasting accuracy during the 2025 test period. ARIMA is retained as an alternative model for future comparison because of its stronger residual diagnostics.

## Final Forecast

The selected model was applied to the complete dataset through December 2025 to generate forecasts for the following five months.

| Month | Forecast ($ Millions) |
|---|---:|
| January 2026 | 5,473 |
| February 2026 | 5,067 |
| March 2026 | 5,437 |
| April 2026 | 5,051 |
| May 2026 | 5,631 |
| **Monthly Average** | **5,331.80** |
| **Total Forecast** | **26,659** |

## Limitations and Future Improvements

- Significant residual autocorrelation in the Seasonal Naive model.
- Unusual sales disruptions during the COVID-19 pandemic.
- Forecast accuracy evaluated using a single 12-month test period.
- External economic and industry variables were not included.

Future improvements include rolling-origin cross-validation, incorporating external predictors, accounting for unusual economic disruptions, and reevaluating model performance as new data becomes available.

## Project Deliverables

- [PowerPoint Presentation](Forecasting%20U.S.%20Electronics%20Store%20Retail%20Sales.pptx) — Detailed analysis, visualizations, model comparisons, residual diagnostics, and forecasting recommendations for a technical audience.
- [Management Report](Management%20Report%20-%20Electronics%20Retail%20Sales.docx) — One-page report summarizing the forecast, methodology, findings, limitations, and business recommendations for management.
- [Original Dataset](Retail%20Sales%20-%20Electronics%20Stores.csv) — Historical monthly retail sales data used throughout the forecasting analysis.

## Data Source

Federal Reserve Bank of St. Louis (FRED): [Retail Sales: Electronics Stores](https://fred.stlouisfed.org/series/MRTSSM443142USN)
