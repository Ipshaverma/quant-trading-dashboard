# Real-Time Quant Trading Dashboard

A powerful, interactive dashboard for quantitative analysis and algorithmic trading strategies. This application allows users to visualize stock market trends, generate trading signals using technical indicators, and backtest strategy performance with risk metrics.

![Dashboard Overview](Dashboard_overview.png)

## 🚀 Features

- **Real-Time Data Fetching**: Integration with `yfinance` to download live and historical stock data.
- **Moving Average Crossover Strategy**: Automated signal generation (Buy/Sell) based on 20-day and 50-day moving averages.
- **Strategy Backtesting**: Detailed analysis of Strategy Returns vs. Market Cumulative Returns.
- **Risk Metrics**: Calculation of crucial trading metrics including:
  - **Sharpe Ratio**: Risk-adjusted performance evaluation.
  - **Maximum Drawdown**: Assessment of strategy downside risk.
- **P&L Tracking**: Visual representation of daily and cumulative Profit & Loss.

![Risk Metrics](Risk_metrices.png)

## 🛠️ Tech Stack

- **[Streamlit](https://streamlit.io/)**: For the interactive web interface.
- **[Pandas](https://pandas.pydata.org/)**: For data manipulation and time-series analysis.
- **[NumPy](https://numpy.org/)**: For mathematical computations.
- **[yfinance](https://github.com/ranaroussi/yfinance)**: For fetching financial data from Yahoo Finance.

## 📈 Strategy Overview: Moving Average Crossover

This dashboard implements a classic **MA Crossover** strategy:
- **Buy Signal (1)**: Generated when the **20-day Moving Average (MA20)** crosses above the **50-day Moving Average (MA50)**.
- **Sell Signal (-1)**: Generated when the **MA20** crosses below the **MA50**.

The strategy backtester calculates returns based on these signals and compares them against a simple "Buy and Hold" market strategy.

![Strategy Returns](Strategy_returns.png)


