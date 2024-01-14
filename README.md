# AQI-Prediction-Model-for-Air-Quality-Assessment-using-PySpark


## Overview

This aims to predict air quality using machine learning techniques. It involves collecting air quality data from various cities, exploring the data, training a machine learning model, and making predictions.

## Dataset

The dataset used in this project contains the following columns:

- `datetime`: Timestamp of the data.
- `main_aqi`: Main Air Quality Index.
- `components_co`, `components_no`, `components_no2`, `components_o3`, `components_so2`, `components_pm2_5`, `components_pm10`, `components_nh3`: Various air quality components.
- `coord_lon`, `coord_lat`: Latitude and longitude of the location.
- `extraction_date_time`: Timestamp when the data was extracted.
- `city_name`: Name of the city.

## Exploratory Data Analysis (EDA)

Performed exploratory data analysis to understand the characteristics of the data. Visualized correlations between different features and checked summary statistics.

## Machine Learning Model

Trained a machine learning model to predict the `main_aqi` using the available features. Used Spark MLlib for training the model.

### Model Performance

Evaluated the model using metrics such as Root Mean Squared Error (RMSE) and R-squared. Achieved good performance on the test set.

## Results

#### Linear Regression Model

- RMSE: 0.37
- R2 Score: 73.4%

#### GBTRegressor Model

- RMSE: 0.08
- R2 Score: 98.7%

### Insights

- Both the models shows high accuracy in predicting air quality.
- Certain features, such as `components_o3` and `components_pm2_5`, have a significant impact on air quality.
- Further analysis could be done to understand the factors affecting air quality in different cities.
