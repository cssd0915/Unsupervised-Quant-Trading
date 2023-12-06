# Unsupervised Quant Trading Strategy

This Jupyter notebook presents an unsupervised machine learning strategy for quantitative trading compared to a traditional SPY Buy & Hold strategy. The notebook covers data extraction, feature calculation, liquidity filtering, return calculation, risk factor analysis, asset clustering, portfolio optimization, and performance visualization.

## Installation

To run this notebook, ensure you have the following Python libraries installed:
- pandas
- numpy
- matplotlib
- yfinance
- pandas_ta
- statsmodels
- scikit-learn
- pypfopt

You can install these packages using pip:
```bash
pip install pandas numpy matplotlib yfinance pandas_ta statsmodels scikit-learn pypfopt
```
## Data
The notebook uses historical data for S&P 500 companies, technical indicators, and Fama-French factors.

## Usage
Execute each cell in order, from top to bottom. The notebook will:

- Download stock data from Yahoo Finance.
- Calculate technical indicators like Garman-Klass Volatility, RSI, Bollinger Bands, ATR, MACD, and Dollar Volume.
- Resample data to a monthly frequency and select the top 150 most liquid stocks.
- Calculate monthly returns over various horizons.
- Download Fama-French factors and compute rolling factor betas.
- Fit a K-Means Clustering algorithm monthly to group similar assets.
- Form portfolios based on Efficient Frontier optimization.
- Compare the unsupervised learning strategy's performance to the SPY Buy & Hold strategy.
- Results

The notebook concludes with a visualization of the cumulative returns of the unsupervised learning strategy against the SPY Buy & Hold returns.
