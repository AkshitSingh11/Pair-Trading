# Pair-Trading

This project implements a pair trading strategy using historical stock price data of Adobe Inc. (ADBE) and Salesforce Inc. (CRM), two large-cap tech companies with similar business fundamentals. The objective is to identify statistically cointegrated pairs and generate mean-reverting trade signals to profit from temporary price deviations.

This notebook performs:
  Data Collection & Visualization: Reads cleaned historical data of ADBE and CRM from a CSV file, visualizes price trends and return distributions.
  Statistical Tests for Pair Selection:
    Pearson Correlation
    Augmented Dickey-Fuller (ADF) Test
    Cointegration p-value (Engle-Granger test)
  Spread Construction: Defines spread as a linear combination of normalized stock prices.
  Z-score Strategy: Computes Z-score of the spread to generate long/short signals when divergence exceeds set thresholds.
  Backtesting: Simulates trade entries/exits, calculates PnL, Sharpe ratio, and visualizes the strategy performance.
