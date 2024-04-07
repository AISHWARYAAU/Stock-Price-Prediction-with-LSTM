# Stock Price Prediction with LSTM

## Overview

This repository contains a Python script to predict stock prices using Long Short-Term Memory (LSTM) neural networks. The stock price data for Apple Inc. (AAPL) is fetched from Yahoo Finance using the `yfinance` library. The dataset includes features like Open, High, Low, Close, Adjusted Close prices, and Volume.

## Requirements

- pandas
- yfinance
- datetime
- plotly
- scikit-learn
- keras

Install the required packages using pip:

```bash
pip install pandas yfinance plotly scikit-learn keras
```

## Data Collection

The script downloads historical stock price data for AAPL from the last 5000 days using the `yfinance` library. The data is then preprocessed to select relevant columns and reset the index.

## Data Visualization

A candlestick chart is plotted using Plotly to visualize the stock price movements over time.

## Data Preprocessing

The dataset is split into features (Open, High, Low, Volume) and the target variable (Close price). The data is then converted to NumPy arrays and reshaped to be compatible with the LSTM model.

## Model Building

An LSTM neural network is constructed using the Keras library. The model architecture consists of two LSTM layers followed by two Dense layers. The model is compiled with the Adam optimizer and Mean Squared Error loss function. It is then trained on the training dataset with a batch size of 1 and 30 epochs.

## Prediction

As a demonstration, the trained LSTM model is used to predict the Close price for a given set of features (Open = 177.089996, High = 180.419998, Low = 177.070007, Volume = 74919600). The predicted Close price is printed to the console.

## Conclusion

This project showcases how LSTM neural networks can be utilized for stock price prediction based on historical data. The model's performance can be further improved by tuning hyperparameters, incorporating additional features, or using more sophisticated architectures.

#images
![image](https://github.com/AISHWARYAAU/Stock-Price-Prediction-with-LSTM/assets/91381783/5680b05f-58aa-4871-aff7-49d95aa0c979)

![image](https://github.com/AISHWARYAAU/Stock-Price-Prediction-with-LSTM/assets/91381783/87ea7d14-f11e-453c-851c-6e9f4c882166)
