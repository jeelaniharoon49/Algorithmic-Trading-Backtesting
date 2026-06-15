###Algorithmic Trading Strategy Backtesting

##Overview

-This project implements and evaluates a Moving Average Crossover trading strategy using historical stock market data from Yahoo Finance.

-The strategy generates buy and sell signals based on the relationship between a 50-day moving average and a 200-day moving average.

-The performance of the strategy is compared against a traditional Buy & Hold investment approach.

#Objectives:
-Download historical stock market data
-Generate trading signals using moving averages
-Backtest strategy performance
-Compare returns against Buy & Hold
-Calculate risk metrics
-Visualize trading signals and portfolio performance

##Technologies Used:

Python
Pandas
NumPy
Matplotlib
Yahoo Finance (yFinance)
Strategy Logic

#Buy Signal Generated when:

50-Day Moving Average > 200-Day Moving Average

#Sell Signal Generated when:

50-Day Moving Average < 200-Day Moving Average

### Risk Metrics
##Sharpe Ratio:

Measures risk-adjusted returns.

##Maximum Drawdown:

Measures the largest portfolio decline from peak value.

##Results:

Metric	Value
Buy & Hold Return	244.00%
Strategy Return	46.01%
Sharpe Ratio	0.48
Maximum Drawdown	-26.58%

##Key Insights:

Buy & Hold outperformed the crossover strategy during a strong bull market.
The strategy reduced market exposure during bearish periods.
Risk-adjusted returns remained positive.
Moving Average strategies can help manage downside risk but may underperform in long-term upward trends.

###Strategy vs Buy & Hold
<img width="1113" height="607" alt="image" src="https://github.com/user-attachments/assets/8ffc2f5e-1df8-407c-a2b0-e857aeb81da1" />
###Buy/Sell Signal Visualization
<img width="1290" height="572" alt="image" src="https://github.com/user-attachments/assets/25d0f085-d920-498e-8cee-a088d4214e04" />

##Future Improvements:

Backtest multiple stocks simultaneously
Add transaction costs
Implement stop-loss mechanisms
Compare alternative trading strategies
Perform portfolio-level backtesting

