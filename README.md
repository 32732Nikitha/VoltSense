# VoltSense
This project focuses on accurately forecasting hourly household energy consumption using machine learning models. By analyzing historical power usage data, the system predicts future consumption to support efficient energy management, reduce waste, and enable smarter grid operations.

--> Objective
To build and compare machine learning models that can predict future energy usage based on historical patterns and time-based features, enabling better planning and automation for smart homes and power distribution systems.

-->Models Implemented
Linear Regression (Baseline) and Random Forest Regressor (Final Model)

--> Dataset
Source: UCI Machine Learning Repository – Individual Household Electric Power Consumption Dataset
Description: Contains power consumption data recorded every minute from 2007 to 2010 for a single household.

--> Methodology

Data Preprocessing:
--Convert date and time to datetime format
--Resample data to hourly intervals
--Handle missing/null values
--Generate lag features (previous 24 hours)
--Extract time-based features (hour, day, etc.)

Model Training:
--Use time-series aware train-test split
--Train and evaluate both Linear Regression and Random Forest models

Evaluation Metrics:
--RMSE (Root Mean Squared Error)
--R² Score (Coefficient of Determination)

-->Results
Random Forest outperforms Linear Regression, particularly in capturing fluctuations and non-linear trends.
Visualizations confirm high alignment between predicted and actual values, especially over short-term windows.

-->Deployment Potential
## Integration into smart home systems for energy monitoring and automation
## City-wide energy demand forecasting for grid balancing
## Power usage alert systems for anomaly detection

-->Future Scope
## Incorporate external data: weather, occupancy, appliance-level usage
## Apply deep learning models like LSTM or GRU for longer-term forecasting
## Develop real-time dashboards or APIs for smart energy applications



