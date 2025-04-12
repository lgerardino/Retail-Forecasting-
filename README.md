# Retail Forecasting Project

## Overview

This project aims to forecast daily demand for a retail business using various time series forecasting models, including ARIMA, SARIMA, and Prophet. The project involves data preparation, exploratory data analysis, model training, cross-validation, and performance evaluation.

The analysis focused on two key questions:

1️⃣ What are the main seasonal trends and demand variations across regions, and how do they affect sales performance?

2️⃣ Which time series forecasting model--ARIMA, SARIMA, or Prophet--provides the most accurate predictions for Units Sold, and how does model performance vary across regions?

To answer these, we conducted a detailed study using historical retail inventory data, applying statistical analysis and machine learning techniques.

## Table of Contents

1. [Data Loading](#data-loading)
2. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
3. [Data Preparation](#data-preparation)
4. [Modeling and Cross Validation](#modeling-and-cross-validation)
5. [Forecasting and Performance Comparison](#forecasting-and-performance-comparison)
6. [Conclusion](#conclusion)


## Data Loading

We import the `pandas` library and install the `seaborn` library. We then attempt to load a CSV file containing retail store inventory data into a DataFrame using `pd.read_csv()`.

## Exploratory Data Analysis (EDA)

### Data Inspection
- Display the first few rows of the DataFrame.
- Examine the shape of the DataFrame.
- Check data types.
- Calculate descriptive statistics for numerical columns.
- Identify missing values.
- Analyze unique values and frequencies for categorical columns.

### Data Visualization
- Plot histograms and boxplots for key variables.
- Analyze correlations between key variables using scatter plots and heatmaps.

## Data Preparation

### Outlier Detection and Removal
- Define functions to detect and remove outliers using the IQR method.
- Analyze and remove outliers for key variables.

### Sales Trend and Variables Relationship Analysis
- Sales tren over time.
- Inventory Levels Across Regions.
- Sales by category, Region, and Weather
- Sales by Region by Season



### Time Series Preparation
- Convert the 'Date' column to datetime format.
- Set the 'Date' column as the index.
- Aggregate the data by day to calculate daily demand.
- Perform ADF test to check dataset stationarity.

## Modeling and Cross Validation

### ARIMA Model
- Define the ARIMA model.
- Perform rolling-origin cross-validation.
- Fit the final ARIMA model on the entire dataset.

### SARIMA Model
- Define the SARIMA model.
- Perform rolling-origin cross-validation.
- Fit the final SARIMA model on the entire dataset.

### Prophet Model
- Define the Prophet model.
- Perform rolling-origin cross-validation.
- Fit the final Prophet model on the entire dataset.

### XGBoost
- Data preparation.
- Define the XGBoost model.
- Perform rolling-origin cross-validation.
- fit the final XGBoost on the entire dataset.

## Forecasting and Performance Comparison

- Generate forecasts using the fitted models.
- Compare the performance of the models using metrics such as RMSE, MAE, and R².
- Create a comparison DataFrame to summarize the results.

## Conclusion

Summarize the findings and insights gained from the analysis and modeling. Discuss the performance of different models and their applicability to retail demand forecasting.

