# Algorithmic Trading with Python
# GOAL: The goal of this program is to predict stock market prices using a Time Series Analysis and ARIMA model, with the output geared towards education on the step-by-step process of the analysis.
# DESCRIPTION: 
#   1. Eduction: Our project aims to provide an educational approach to trading strategies using a Time Series Analysis. The program's output will be presented in an educative manner, showing step-by-step how the ARIMA model works, how the predictions are made, and how the trading strategy operates. The output will also include visualizations of the data and results, making it easier to understand for users who are new to Time Series Analysis and trading strategies.
#   2. ARIMA Model: The core of our program will be based on the ARIMA (AutoRegressive Integrated Moving Average) Model, which is a statistical model used for time series analysis and forecasting. We will first gather data from the stock market using pandas-datareader and create a pandas DataFrame object. We will then implement the ARIMA model and predict future stock prices based on the time series analysis. Our program will also focus on trading strategies by using the ARIMA model's predictions to make buy or sell decisions. We will create a trading strategy that buys stocks when the predicted price is higher than the current price and sells when the predicted price is lower than the current price.
#   3. Trading Strategies: If time allows, our program will also handle trading strategies other than the ARIMA model, some of which include momentum trading and MACD.
#   4. If time allows, our program will backtest the program over a period of time using historical data to verify the success of our trading strategy.
# CODE: 
#   Alpaca_demo.py: The code utilizes the Alpaca trading API to interact with the stock market. It creates a client object using an API key, handles buying orders, and extracts information about the client’s portfolio
#   config.py: This code interacts with the stock market and fetches the user’s account information to buy shares of a stock. 
#   lumibot_buy_hold.py: This code involves backtesting a trading strategy using the Lumibot library. The specific trading strategy implemented in this code is a "buy and hold" strategy, where the user buys shares and holds onto them for the entire trading period. The Alpaca broker is used for live trading, while YahooDataBacktesting is used for backtesting. 
#   lumibot_swing_high.py: This Python script implements the "Swing High" trading strategy, which uses a moving window to buy a security when it appears to be in a bullish trend and sell it when it starts to reverse. The script uses the Alpaca brokerage API and the lumibot library for backtesting and live trading.
#   portfolio.py: This code uses the quantstats library to create a portfolio object from a dictionary of asset weights and generates two plots of the portfolio's earnings and monthly returns. The plots are saved as files in the "output" folder. The print() statement is commented out.
#   single_stock.py: The code uses the quantstats library, calculates various statistics such as Sharpe ratio, CAGR, and maximum drawdown using quantstats and pandas dataframe methods. It extends pandas with qs.extend_pandas() function and outputs the results.
#   strategy.py: The code imports various libraries such as datetime, dateutil, os, pandas, pandas-datareader, numpy, quantstats, and webbrowser. It defines a function called "ma_cross_strategy()" that takes four arguments and returns a pandas series object. The code calls the "ma_cross_strategy()" function with specific parameters and stores the result in a variable named "gld_cross". It then downloads return data for the "GLD" ETF over the past three years and generates a report comparing the strategy returns with the actual returns using the quantstats library. 
#   ts_demo.py: The code imports necessary libraries and retrieves unemployment data from OpenBB API. It then processes the data by calculating rolling mean and standard deviation and decomposing the time series into trend, seasonal, and residual components using the seasonal_decompose and STL() from statsmodels.tsa.seasonal. Finally, it plots and displays the decomposed time series with the title.
# RESEARCH: Libraries: Research was done on the smodels.tsa.stattools and pmdarima libraries to implement the ARIMA model https://colab.research.google.com/drive/12erf5mqimQEFrXFZSsP3I3OKk6wr7Ewi?usp=sharing
# FUTURE ENHANCMENTS:
#   User Interactivity: Allow the user to input more parameters, such as the range of years for unemployment or allow the user to create their own strategy. 
#   Increase Analysis Techniques: More analysis techniques could be used, like GDP, inflation rate, or clustering
#   Visualization: Currently, the only visualization is that of a time series, but more could be included like pie charts or bar charts. 




