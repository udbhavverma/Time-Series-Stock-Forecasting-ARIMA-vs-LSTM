This project provides an in-depth comparison between classical statistical models (ARIMA/GARCH) and deep learning models (LSTM) for the notoriously difficult task of stock price prediction. It serves as a comprehensive exploration of the methodologies, challenges, and realistic outcomes of financial forecasting.

Project Overview
The project follows a structured workflow:

Data Pipeline: Fetched over 10 years of daily stock data for Apple (AAPL) using the yfinance API.

Statistical Analysis: Conducted rigorous time-series analysis, including testing for stationarity with the Augmented Dickey-Fuller (ADF) test.

Feature Engineering: Enriched the dataset with 12+ technical indicators (e.g., RSI, MACD, Bollinger Bands) using the pandas-ta library to provide richer context for the deep learning model.

Modeling: Implemented and trained both an ARIMA model (validated with walk-forward validation) and a multi-feature LSTM network.

Hyperparameter Tuning: Utilized KerasTuner to systematically search for an optimal LSTM architecture and learning rate.

Comparative Analysis: Performed a head-to-head comparison of the models based on Root Mean Squared Error (RMSE) and Directional Accuracy.

Key Findings
The analysis yielded a realistic and insightful outcome: neither model achieved a directional accuracy significantly above 50%, demonstrating the Efficient Market Hypothesis in practice. The project highlights that while historical data is useful, predicting stock movements requires more complex features, and this repository serves as a robust baseline for such future work.

Technologies Used
Python

Pandas & NumPy for data manipulation

yfinance & pandas-ta for data and feature retrieval

statsmodels & pmdarima for ARIMA modeling

TensorFlow & Keras for the LSTM network

KerasTuner for hyperparameter optimization

scikit-learn for data scaling and metrics

Matplotlib for visualization
