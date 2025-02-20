# Demand Forecasting with LSTM Neural Networks

### Overview

This project implements a demand forecasting model using Long Short-Term Memory (LSTM) neural networks to predict product sales based on historical data. The model leverages time series data, including lag features, rolling averages, and inventory levels, to forecast daily units sold. The goal is to optimize inventory management, reduce stockouts, and provide actionable insights for decision-making in retail.

### Objective

The project aims to provide actionable insights for optimizing inventory, reducing stockouts, and enhancing decision-making in retail.

### Dataset

This dataset provides synthetic yet realistic data for analyzing and forecasting retail store inventory demand. It contains over 73000 rows of daily data across multiple stores and products, including attributes like sales, inventory levels, pricing, weather, promotions, and holidays.

### Key Features:

- Date: Daily records from [start_date] to [end_date].
- Store ID & Product ID: Unique identifiers for stores and products.
- Category: Product categories like Electronics, Clothing, Groceries, etc.
- Region: Geographic region of the store.
- Inventory Level: Stock available at the beginning of the day.
- Units Sold: Units sold during the day.
- Demand Forecast: Predicted demand based on past trends.
- Weather Condition: Daily weather affecting sales.
- Holiday/Promotion: Indicators for holidays or promotions.

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

### Challenges Addressed:

- Data Preprocessing: The data is cleaned and aggregated by store and product to handle missing values and ensure consistency.
- Feature Engineering: Key features like lag features, rolling averages, seasonal features (month, weekday, weekend), and weather conditions are created to improve the accuracy of the forecast.
- Modeling: LSTM is used to capture the temporal dependencies of sales data, providing predictions that can be used to optimize inventory levels and improve demand forecasting accuracy.

### Results:

- LSTM RMSE: 108.26
- LSTM MAE: 89.35

Achieved an RMSE of 108.26 and an MAE of 89.35, indicating a reasonable prediction accuracy.

### Key Findings:

- Both RMSE and MAE indicate that the model has a reasonable performance but isn’t highly accurate yet. These values suggest that the model’s predictions are off by a significant amount, which may be expected for a complex problem like predicting sales over time with various influencing factors.

- To assess model performance more thoroughly, you could compare these values with other models (e.g., traditional statistical models or simpler machine learning algorithms) to determine if the LSTM provides a meaningful improvement.

- Depending on the business context, these errors may be acceptable, but if high accuracy is needed for inventory planning, for example, further model tuning, feature engineering, or additional data might be necessary to improve these metrics.

### Future Work:

- Fine-tune the LSTM architecture (number of layers, units).
- Add more features like competitor pricing, marketing spend, etc.
- Test different models such as GRU or ARIMA for comparison.

### Source

Dataset: [Retail Store Inventory Forecasting Dataset on Kaggle](https://www.kaggle.com/datasets/anirudhchauhan/retail-store-inventory-forecasting-dataset/data)
