# Dreamers-Challenge
# Cryptocurrency Price Prediction Challenge

This repository contains the code and documentation for the Cryptocurrency Price Prediction Challenge. The goal of this challenge is to predict whether the price of a cryptocurrency will increase or decrease in the next minute based on historical price data.

## Dataset

The dataset includes minute-by-minute price information of one cryptocurrency. It is split into two files:

- `train.csv`: Training data with features and target.
- `test.csv`: Test data without the target.

Each row in the dataset represents a minute of trading activity and includes the following columns:

- `timestamp`: The timestamp for the minute.
- `open`: The opening price.
- `high`: The highest price during the minute.
- `low`: The lowest price during the minute.
- `close`: The closing price at the end of the minute.
- `volume`: The number of units traded during the minute.
- `quote_asset_volume`: The total value of the traded units in USDT during the minute.
- `number_of_trades`: The number of trades that occurred.
- `taker_buy_base_volume`: The amount of the crypto asset bought by takers.
- `taker_buy_quote_volume`: The value of the asset bought by takers in USDT.

## Models Used

We employ a Random Forest Classifier to predict the price movement direction due to its ability to handle non-linear data and provide feature importance metrics. The model training involves:

- Feature engineering to calculate moving averages, RSI, and other technical indicators.
- Handling missing values with imputation.
- Hyperparameter tuning for optimization.

## Setup and Installation

1. Clone this repository.
2. Install required Python packages:
