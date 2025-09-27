# ARIMA-MODEL
“An ARIMA-based statistical arbitrage (pairs trading) model that forecasts the spread between two assets. Includes data fetching, spread analysis, ACF/PACF tests, residual diagnostics, and future spread predictions with confidence intervals.”

📊 ARIMA Model for Statistical Arbitrage (Pairs Trading Strategy)

This project applies an ARIMA (AutoRegressive Integrated Moving Average) model to Statistical Arbitrage (StatArb), focusing on pairs trading. Instead of only spotting when assets move apart, this model goes a step further — it actually forecasts the spread between two assets to predict when they may come back together.

🌍 What is Statistical Arbitrage?

Statistical Arbitrage is about trading relationships instead of individual assets.

Think of two related stocks (like GBP/AUD and GBP/JPY forex pairs).

Most of the time, they move in sync.

But sometimes, one gets ahead while the other lags — creating a spread.

Usually, this spread doesn’t last forever and returns to normal.

The idea:

Sell the one that’s too high.

Buy the one that’s too low.

Profit when the spread comes back to balance.

This makes it a market-neutral strategy — it doesn’t matter if markets are going up or down, only how the two assets move relative to each other.

📌 What This Project Does

This notebook uses an ARIMA model to analyze and forecast the spread between two assets. Here’s how it works step by step:

Collects Data → Pulls historical price data from Yahoo Finance.

Calculates Spread → Finds the difference between the two selected assets.

Plots & Tests → Shows the spread, plus Autocorrelation (ACF) and Partial Autocorrelation (PACF) to check if forecasting is possible.

Fits ARIMA Model → Builds a statistical model to capture patterns in the spread.

Residual Analysis → Checks if the model fits well by analyzing the leftover errors.

Forecasting → Predicts the spread for the next few days and shows it with confidence intervals.

Interactive Widgets → Lets you choose any two assets and date range, then run the analysis with one click.

🎯 Why This is Useful

Goes beyond detection → Unlike Z-Score, which only shows when assets diverge, ARIMA actually forecasts future spreads.

Decision support → Traders can anticipate when the spread might narrow or widen, making entry/exit timing smarter.

Educational value → Great way to learn time series forecasting applied to finance.

Hands-on analysis → Easy to test with different assets, periods, and strategies.

🛠 Tools & Libraries

Python (Google Colab) – main language

yfinance – fetching market data

Pandas, NumPy – handling data

Matplotlib, Seaborn – visualization

Statsmodels (ARIMA, ACF, PACF) – time series modeling

ipywidgets – interactive asset/date selection


![image alt](https://github.com/AryanSahay1/ARIMA-MODEL/blob/main/download%20(1).png?raw=true)
![image alt](https://github.com/AryanSahay1/ARIMA-MODEL/blob/main/download%20(2).png?raw=true)
![image alt](https://github.com/AryanSahay1/ARIMA-MODEL/blob/main/Screenshot%202025-09-27%20122424.png?raw=true)
![image alt](https://github.com/AryanSahay1/ARIMA-MODEL/blob/main/download%20(4).png?raw=true)
![image alt](https://github.com/AryanSahay1/ARIMA-MODEL/blob/main/download%20(7).png?raw=true)



👤 Author: Aryan Sahay
⚠️ Disclaimer: This project is for educational and research purposes only. It is not financial advice.
