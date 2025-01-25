# salesSense-Pharmacy-Sales-Forecaster-
We are developing an inventory management model using a medical pharmacy dataset. Trained on historical sales data, our model predicts future sales of various medicines, helping to optimize stock levels, minimize wastage, and ensure availability of high-demand items for better inventory efficiency.

# Medical Inventory Analysis and Forecasting

This project involves predictive modeling for medical inventory sales data using machine learning and time-series forecasting techniques. The primary goal is to analyze weekly sales data and build models to forecast future trends.

## Key Models

### 1. ARIMA (AutoRegressive Integrated Moving Average)
- **Purpose**: Time-series forecasting.
- **Implementation**: 
  - Uses the `statsmodels` library to build and fit an ARIMA model.
  - Handles seasonality and trends in the data.

### 2. XGBoost Regressor
- **Purpose**: Predict future sales using a gradient-boosted decision tree model.
- **Implementation**:
  - Uses the `XGBRegressor` from the `xgboost` library.
  - Trains the model on lagged features derived from historical sales data.

### 3. LSTM (Long Short-Term Memory)
- **Purpose**: Neural network-based approach for time-series prediction.
- **Implementation**:
  - Built using `tensorflow.keras` with a `Sequential` model.
  - Incorporates layers like LSTM, Dense, and Dropout to capture temporal dependencies and reduce overfitting.
  - Data is normalized using `MinMaxScaler` to improve learning efficiency.

## Evaluation Metrics
- **Mean Squared Error (MSE)**: Measures the average squared difference between predicted and actual values.
- **Mean Absolute Percentage Error (MAPE)**: Quantifies prediction accuracy as a percentage.

## Dependencies
The project relies on the following Python libraries:
- `pandas`: Data manipulation and preprocessing.
- `numpy`: Numerical computations.
- `matplotlib`: Data visualization.
- `statsmodels`: Time-series analysis and forecasting.
- `xgboost`: Machine learning for regression.
- `tensorflow.keras`: Neural network modeling.
- `scikit-learn`: Data preprocessing and evaluation metrics.
