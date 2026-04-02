# Time Series Analysis of EU Electricity Consumption

This project analyzes monthly electricity consumption data for selected European countries using time series techniques in R.

## Overview

The analysis focuses on Spain, Ireland, and Sweden, comparing their electricity consumption patterns and evaluating different forecasting models.

This project was originally developed as part of a university course in Time Series Modeling and Forecasting and later refined.

## Objectives

- Explore time series patterns (trend and seasonality)
- Compare classical and STL decomposition methods
- Evaluate forecasting performance using ETS and ARIMA models
- Assess model adequacy through residual diagnostics

## Methods

The analysis follows the workflow below:
- **Exploratory Analysis:** Visualization of time series and identification of trend and seasonal patterns
- **Decomposition:** Classical (additive and multiplicative) and STL decomposition with different smoothing parameters
- **Model Selection:** The data is split in training and test sets (training until 2022 and testing on 2023), model comparison is based on RMSE
- **Forecasting:** ETS and ARIMA models are used and forecasts are compared against the test data
- **Model Evaluation:** Error measures such as RMSE, MAE, MAPE are calculated and residual diagnostics (such as Ljung–Box test) are performed

## Key Insights

- All countries exhibit strong seasonal patterns
- Spain and Sweden show a slight downward trend, while Ireland shows an upward trend
- ARIMA performs best for Spain and Ireland
- ETS performs better in Sweden in terms of accuracy, but ARIMA shows better residual behavior
- Forecast accuracy alone is not sufficient - residual diagnostics are essential

## Tools & Libraries

- R
- forecast
- fpp2
- ggplot2
- dplyr

## Project Structure

```

├── data/
│   └── electricity_EU27.RData
├── analysis.Rmd
└── README.md
```


## How to Run

1. Open the `.Rmd` file in RStudio
2. Make sure required packages are installed
3. Knit the document to HTML

## Author

Lara Pereira
