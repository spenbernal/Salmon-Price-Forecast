# Salmon Price Forecasting: Time Series vs. Regression-Based Approaches

## Project Description

In this project, I forecast salmon prices using both time series models and regression-based techniques. The goal is to compare the performance of these approaches and determine which method is best suited for accurate and reliable long-term forecasting. The dataset includes monthly salmon prices along with engineered features to capture seasonality and lag effects.

## Project Objectives

Explore different time series forecasting models such as FB Prophet and LSTM.

Implement regression-based techniques like Polynomial Regression, Gradient Boosting, and Random Forest.

Compare model performance using key evaluation metrics (RMSE, R² score).

Provide recommendations on the best forecasting strategy.

## Dataset

The dataset contains salmon prices from 1994 to 2024 with additional features:

Date: Date of the price.

Change: percent change from previous month of price.


## Models Used

### Time Series Models

FB Prophet: Handles seasonality and change points.

LSTM (Long Short-Term Memory): A neural network model that captures long-term dependencies in sequential data.

### Regression-Based Models

Polynomial Regression: Captures non-linear relationships between features and the target variable.

Gradient Boosting Regressor: A powerful ensemble method that captures complex patterns in the data.

Random Forest Regressor: Robust to noise and effective at handling non-linearities.

## Feature Engineering

For the regression-based models, the following features were created to capture patterns in the data:

Lag Features: Capturing the prices from the previous 1, 2, and 3 months.

Rolling Average: Smoothing out short-term fluctuations with a 3-month rolling average.

Seasonal Features: Using sine and cosine transformations to represent the cyclical nature of months.

## Evaluation Metrics

The models were evaluated using:

Root Mean Squared Error (RMSE): Measures the average error in dollars.

R² Score: Indicates how well the model explains the variance in the data.

## Key Insights

Time Series Models are effective for short-term forecasts and automatically account for seasonality.

Regression-Based Techniques are more flexible and better suited for long-term forecasting, especially when additional external features are available.

Feature engineering, particularly lag features and rolling averages, is essential for regression models.

## Conclusion

For short-term forecasting (up to 12 months), FB Prophet or SARIMA are suitable choices. However, for long-term forecasting (over 1 year), Gradient Boosting or LSTM models are recommended as they better capture non-linear trends and long-term dependencies.

This project demonstrates how different forecasting approaches can yield varied results based on the time horizon and nature of the data. By comparing time series models and regression-based techniques, I provide actionable insights into the best methods for predicting salmon prices.

## Next Steps

Experiment with more advanced hyperparameter tuning.

Incorporate additional external factors (e.g., weather, economic indicators) to improve model performance.

Explore ensemble models combining the strengths of both time series and regression approaches.



