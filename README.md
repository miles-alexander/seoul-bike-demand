# Predicting Seoul Bike Rental Demand 🚲

## Overview

This project uses machine learning to forecast hourly bike rental demand in Seoul based on weather and time-based variables. The goal is to improve operational efficiency in bike-sharing programs by anticipating high and low usage periods.

This work is intended to inform resource planning and highlight how open data can drive smarter urban mobility decisions.

## Author

[@miles-alexander](https://github.com/miles-alexander)

---

## Research Questions

      1. How does temperature affect hourly bike rental demand?
      2. What time-of-day trends influence usage patterns?
      3. Are holidays and seasons significant predictors of demand?
      4. Which model best predicts short-term rental fluctuations?

---

## Approach

**Data Cleaning:** Addressed missing values, standardized date formatting, and normalized weather features.

**Exploratory Data Analysis (EDA):** Used line plots, heatmaps, and correlation matrices to identify trends.

**Feature Engineering:** Created temperature bands and hourly average rental metrics.

**Modeling:** Trained Random Forest, Gradient Boosting, Linear Regression, and ARIMA time-series models.

**Evaluation:** Compared performance using RMSE and MAE.

---

## Data Sources & Preparation

This project uses a public dataset available on the UCI Machine Learning Repository:

* **Dataset:** Seoul Bike Sharing Demand
* **URL:** https://archive.ics.uci.edu/ml/datasets/Seoul+Bike+Sharing+Demand
* **Time Period:** January 2017 to December 2018
* **Target Variable:** Rented Bike Count

---

## How to Use

* Download the dataset from the UCI repository.

* Open the Jupyter notebook file: Predicting Seoul Bike Rental Demand.ipynb

* Ensure required libraries (pandas, matplotlib, sklearn, statsmodels) are installed.

* Run all cells in order to see preprocessing, modeling, and results.

---

## Preprocessing & Cleaning Steps
      Converted date format to DD/MM/YYYY
      Normalized numerical features
      Handled missing values by column-wise mean imputation
      Created new columns: AvgHourlyRental, TempBand

---

## Tools & Libraries
* Python
* pandas
* matplotlib
* seaborn
* scikit-learn
* statsmodels

## Key Findings

**Commute Hours:** Rentals spike around 8am and 6pm.

**Temperature:** Usage is highest on mild to warm days.

**Holidays:** Significantly lower demand compared to weekends.

**Model Accuracy:** Random Forest and Gradient Boosting yielded the lowest error.

---

## Limitations

**No station-level data:** predictions are not location-specific.

**Only two years of data:** limits long-term trend detection.

**No rider type labels:** can’t distinguish between commuters and casual users.

---

## Conclusion

This project highlights the predictive value of environmental and temporal data in managing urban bike-share systems. The findings support the development of tools that anticipate demand and improve service delivery.

---

## Future Work

* Add geospatial data to model station-level demand.
* Integrate real-time weather API feeds.
* Deploy predictions in an interactive dashboard for operations teams.
