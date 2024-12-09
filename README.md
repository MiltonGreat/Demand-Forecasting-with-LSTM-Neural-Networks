# Demand-Forecasting-with-LSTM-Neural-Networks

### Overview

This project implements a demand forecasting model using Long Short-Term Memory (LSTM) neural networks to predict product sales based on historical data. The model leverages time series data, including lag features, rolling averages, and inventory levels, to forecast daily units sold.

### Objective

The project aims to provide actionable insights for optimizing inventory, reducing stockouts, and enhancing decision-making in retail.

### Dataset

This dataset provides synthetic yet realistic data for analyzing and forecasting retail store inventory demand. It contains over 73000 rows of daily data across multiple stores and products, including attributes like sales, inventory levels, pricing, weather, promotions, and holidays.

### Workflow

##### Data Preprocessing:
- Handling missing values.
- Aggregating sales data by Date, Store ID, and Product ID.
- Feature engineering with lag features, rolling averages, and seasonal patterns.

##### Exploratory Data Analysis (EDA):
- Visualizations of sales trends, inventory levels, and relationships between key variables.

##### LSTM Model:
- Multilayer LSTM architecture with dropout for regularization.
- Optimized using MinMaxScaler for feature scaling and early stopping to prevent overfitting.
- Evaluation metrics: Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE).

##### Performance:
- Achieved an RMSE of 108.26 and an MAE of 89.31, indicating a reasonable prediction accuracy.

### Results

 - RMSE: 108.26
 - MAE: 89.31

### Source

https://www.kaggle.com/datasets/anirudhchauhan/retail-store-inventory-forecasting-dataset/data
