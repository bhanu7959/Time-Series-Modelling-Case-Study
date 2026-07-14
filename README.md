# German Electricity Demand Forecasting

## Project Overview

This project investigates the forecasting of German electricity demand using statistical, machine learning and deep learning techniques. The objective is to compare different forecasting models and determine which approach provides the most accurate predictions for electricity demand.

The study uses publicly available German electricity demand data from the **Open Power System Data (OPSD)** project together with historical Berlin temperature data obtained from the **Open-Meteo Historical Weather API**.

---

## Dataset

### Electricity Demand
- **Source:** Open Power System Data (OPSD)
- **Country:** Germany (DE)
- **Period:** January 2015 – October 2020
- **Original Frequency:** Hourly

Dataset:
https://data.open-power-system-data.org/time_series/

### Temperature Data
- **Source:** Open-Meteo Historical Weather API
- **Location:** Berlin, Germany

API Documentation:
https://open-meteo.com/en/docs/historical-weather-api

---

## Project Workflow

The project consists of the following stages:

### Part 1
- Data collection
- Data cleaning
- Weekly aggregation
- Exploratory Data Analysis
- Stationarity testing

### Part 2
Benchmark forecasting models:

- Mean Forecast
- Naïve Forecast
- Seasonal Naïve Forecast
- Drift Forecast

### Part 3
SARIMA forecasting

- Parameter tuning using AIC
- Residual diagnostics
- Two-year forecast
- Confidence intervals

### Part 4
SARIMAX forecasting

- Weekly Berlin temperature
- Exogenous variables
- Conditional forecasting

### Part 5
Feature-based forecasting

Random Forest Regressor

Features include:

- Lag variables
- Rolling averages
- Temperature
- Calendar features

### Part 6
Deep Learning

Long Short-Term Memory (LSTM)

- Hourly electricity demand
- One-week lookback window
- Early stopping
- Model evaluation

---

## Evaluation Metrics

All forecasting models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Symmetric Mean Absolute Percentage Error (sMAPE)

---

## Libraries Used

- Python
- Pandas
- NumPy
- Matplotlib
- Statsmodels
- Scikit-learn
- TensorFlow / Keras

---

## Results

The forecasting models were compared to determine whether more advanced statistical and deep learning models improved upon the Seasonal Naïve benchmark.

The report discusses:

- Forecast accuracy
- Model complexity
- Interpretability
- Operational suitability

---

## References

- Open Power System Data
- Open-Meteo
- Hyndman & Athanasopoulos – Forecasting: Principles and Practice
- Box, Jenkins & Reinsel – Time Series Analysis

