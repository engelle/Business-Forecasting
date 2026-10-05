# Assignment #4 - Forecasting Models

## Overview

For this assignment, I applied several forecasting methods to the Retail Sales: Electronics Stores time series used in Assignment #3. The dataset contains monthly U.S. electronics store sales from January 2016 through December 2025.

The goal of this assignment was to compare different forecasting methods and evaluate how well they capture patterns in the data, particularly the monthly seasonality.

## Forecasting Methods

The following methods were explored:

- Mean Forecast
- Naive Forecast
- Random Walk
- Random Walk with Drift
- Seasonal Naive Forecast
- Moving Averages (MA5 and MA9)
- ETS
- Holt-Winters
- Simple Exponential Smoothing

## Model Evaluation

To compare forecasting accuracy, the data was divided into a training set containing observations from 2016 through 2024 and a test set containing the 12 months of 2025.

Root Mean Squared Error (RMSE) was used as the accuracy measure. The Seasonal Naive model produced the lowest RMSE of **196.07**, followed by ETS with an RMSE of **261.66** and Holt-Winters with an RMSE of **278.98**.

Based on RMSE, the Seasonal Naive model was the most accurate model for this dataset. This suggests that the recurring yearly seasonal pattern is particularly important when forecasting monthly electronics store sales.

## Dataset

- **Dataset:** Retail Sales: Electronics Stores
- **FRED Series ID:** MRTSSM443142USN
- **Time Period:** January 2016 - December 2025
- **Frequency:** Monthly
- **Number of Observations:** 120
- **Units:** Millions of Dollars
- **Seasonal Adjustment:** Not Seasonally Adjusted
- **Geographic Coverage:** United States

## Files

- `Assignment 4 - Forecasting Models.Rmd` - R Markdown source file containing the analysis and R code
- `Assignment-4---Forecasting-Models.html` - Knitted HTML report containing the code, output, graphs, and explanations
- `Retail Sales - Electronics Stores.csv` - Dataset used for the analysis

## Tools

- R
- RStudio
- forecast package
- ggplot2 package
