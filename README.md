# Project Overview
This project builds and backtests an algorithmic trading strategy on Apple (AAPL) stock using a Moving Average Crossover approach, comparing its performance against a passive Buy & Hold strategy.

# Business Problem
Investors and traders need a systematic, rule-based approach to decide when to enter and exit a position.
This project answers the question: *"Can a data-driven trading strategy outperform simply holding a stock?"*

# Dataset
- Ticker: AAPL (Apple Inc.)
- Source: Yahoo Finance via `yfinance`
- Period: 2020–2025 (5 years of daily price data)
- Feature used: Adjusted Close Price

# Strategy
**Moving Average Crossover (MA50 / MA200)**
- Buy Signal — 50-day MA crosses above 200-day MA (Golden Cross)
- Sell Signal — 50-day MA crosses below 200-day MA (Death Cross)

# Performance Metrics

| Metric | Description |
|---|---|
| Cumulative Return | Total return of strategy vs. buy & hold over 5 years |
| Sharpe Ratio | Risk-adjusted return of the strategy |
| Maximum Drawdown | Largest peak-to-trough loss during the period |

## Strategy vs. Buy & Hold
<img width="1106" height="603" alt="image" src="https://github.com/user-attachments/assets/3d34f997-7033-4303-b869-95caf8c1fd55" />


## Buy & Sell Signals on Price Chart
<img width="637" height="492" alt="image" src="https://github.com/user-attachments/assets/ca38792d-b8e9-40b5-ad97-6bb99484837d" />

Results

MetricStrategyBuy & HoldCumulative Return46.01%244.0%Sharpe Ratio0.480.94Maximum Drawdown-26.58%-31.43%

## Key Takeaway
Simple rule-based strategies do not always beat buy & hold — especially on trending growth stocks. This project demonstrates how to measure that honestly using cumulative returns, Sharpe ratio, and drawdown rather than just eyeballing a chart.

## Technologies Used
- Python
- Pandas
- NumPy
- Matplotlib
- yfinance
- Google Colab

## Author
Haroon Jeelani
