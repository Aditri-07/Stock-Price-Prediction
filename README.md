# Stock Price Prediction with LSTM

## Overview

This project aims to predict the closing prices of Google (GOOG) stock using a Long Short-Term Memory (LSTM) neural network. By leveraging historical stock prices and engineered features, the model provides insights into future stock price trends.

## Project Purpose

The primary goal of this project is to implement a robust machine learning model that can accurately predict stock prices. This can assist investors and financial analysts in making informed decisions based on predicted stock trends.

## Functionality

1. **Data Loading**: Load historical stock price data from a CSV file.
2. **Preprocessing**: Clean and transform the data for modeling.
3. **Feature Engineering**: Generate lagged features to capture temporal dependencies.
4. **Model Training**: Train an LSTM model on the preprocessed data.
5. **Prediction**: Generate predictions for training, validation, and test datasets.
6. **Visualization**: Plot the predicted prices against the actual stock prices for evaluation.

## Technologies Used

- **Python**: Programming language used for the entire project.
- **Pandas**: Data manipulation and analysis.
- **NumPy**: Numerical computing.
- **Matplotlib**: Data visualization.
- **Scikit-learn**: Data preprocessing and evaluation metrics.
- **TensorFlow**: Deep learning framework for building and training the LSTM model.

## Technical Details

### Data Preprocessing

- Loaded historical stock data from `GOOG.csv`.
- Converted date strings to datetime objects.
- Engineered lagged features (`close_lag1`, `close_lag7`) to capture historical trends.
- Normalized features using `MinMaxScaler`.

### Model Architecture

- **LSTM Layer**: Captures temporal dependencies in the data.
- **Dense Layers**: Added for further processing and final prediction.
- **Optimizer**: Adam optimizer for efficient training.
- **Loss Function**: Mean squared error (MSE) to minimize prediction error.

### Model Training

- Split data into training, validation, and test sets (80% training, 10% validation, 10% testing).
- Trained the model for 50 epochs with a batch size of 32.
- Evaluated model performance using mean absolute error (MAE).

### Visualizations

- Plotted training, validation, and test predictions against actual stock prices.
- Used combined dates for clear and comprehensive visualization.

## Examples of Use

- **Investment Strategy**: Use the model to predict future stock prices and make informed investment decisions.
- **Financial Analysis**: Analyze stock price trends and generate reports for financial analysis.
- **Algorithmic Trading**: Integrate the model with trading algorithms for automated trading strategies.
