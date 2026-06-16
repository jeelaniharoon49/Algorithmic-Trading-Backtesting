Algorithmic Trading & Backtesting — Moving Average Crossover

A Python project that builds and backtests a simple algorithmic trading strategy on Apple (AAPL) stock, comparing its performance against a passive buy & hold approach.

The Question This Project Answers


"When should I buy and sell?"



Instead of holding a stock indefinitely, this project tests whether a rule-based strategy — buy when short-term momentum is rising, sell when it falls — can be a smarter approach.

Strategy

Moving Average Crossover (MA50 / MA200)


Buy signal — when the 50-day moving average crosses above the 200-day moving average (golden cross)
Sell signal — when the 50-day moving average crosses below the 200-day moving average (death cross)
Data: AAPL daily prices from 2020 to 2025 via yfinance

What the Project Does


Downloads 5 years of AAPL price data
Calculates 50-day and 200-day moving averages
Generates buy/sell signals based on the crossover
Computes daily strategy returns vs. market (buy & hold) returns
Calculates cumulative returns, Sharpe ratio, and maximum drawdown
Plots strategy vs. buy & hold performance
Plots buy/sell signal markers on the price chart


Performance Metrics

MetricDescriptionCumulative ReturnTotal return of the strategy vs. buy & hold over 5 yearsSharpe RatioRisk-adjusted return of the strategyMaximum DrawdownLargest peak-to-trough loss during the period

Visualizations

1. Strategy vs. Buy & Hold — Cumulative Returns
Compares how ₹1 invested in the MA crossover strategy grew vs. simply holding AAPL.

2. Moving Average Crossover Signals
Shows AAPL price with buy signals (▲) and sell signals (▼) marked at each crossover point.

Tech Stack

Python · pandas · numpy · yfinance · matplotlib

Key Takeaway

Simple rule-based strategies don't always beat buy & hold — especially on trending growth stocks like AAPL. This project demonstrates how to measure that honestly using cumulative returns, Sharpe ratio, and drawdown rather than just eyeballing a chart.
