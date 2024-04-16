# ValueInvestor 

# Background:

The goal is to establish a robust intelligent system to aid the value investing efforts using stock market data, the investment decisions should be based on intrinsic value of companies and not on the basis of daily market volatility. The profit realization strategy typically involves weekly, monthly and quarterly performance of stocks we buy or hold.

# Data Description:

Set of portfolio companies trading data from emerging markets including 2020 Q1-Q2-Q3-Q4 2021 Q1 stock prices. Each market's operating days varies based on the country of the company and the market the stocks are exchanged. Predict with the 2021 Q1 data.

# Goal(s):

* Predict stock price valuations on a daily, weekly and monthly basis.
* Recommend BUY, HOLD, SELL decisions.
* Maximize capital returns, minimize losses.
* Ideally a loss should never happen. Minimize HOLD period.
* Evaluate on the basis of capital returns. Use Bollinger Bands to measure the system effectiveness.

# Methodology:

* After trying different time series forecasting models for our initial dataset focused on Russia's Sberbank Stocks, LSTM model is the best fit.

![image](https://github.com/53KIbGcAqz0Gokmj/DeYOPOp5UPd8ZajM/assets/143815258/31425613-e0e3-4790-9c48-666d5fb10ebe)

![image](https://github.com/53KIbGcAqz0Gokmj/DeYOPOp5UPd8ZajM/assets/143815258/5c8780e4-22b8-4770-b895-3651a40bf9f3)

Evaluate the model on the whole data and predict 20 months into the future (till the end of next year) 

![image](https://github.com/53KIbGcAqz0Gokmj/DeYOPOp5UPd8ZajM/assets/143815258/e6269803-319c-4ea8-9df8-cef6ab5b2ef2)


![image](https://github.com/53KIbGcAqz0Gokmj/DeYOPOp5UPd8ZajM/assets/143815258/e767734f-b751-4c6e-b781-540b260511dc)


1. Exponential Smoothing (MAPE: 2.69%): While Exponential Smoothing is straightforward to implement and captures general trends, its forecasting performance diminishes with intricate trends, complex patterns, or long-term dependencies.
2. FB Prophet (MAPE: 16.83%): Designed to handle missing data and outliers effectively, FB Prophet can also accommodate seasonality and holidays. However, it's not most suitable choice for rapidly changing trends and complex patterns.
3. ARIMA (AutoRegressive Integrated Moving Average) (MAPE: 2.91%): ARIMA performs well with linear trends and stationary time series, and it can capture seasonality through differencing. But, its efficacy diminishes when faced with non-linear patterns, making it less suitable for forecasting complex trends.
4. LSTM (Long Short-Term Memory) (MAPE: 1.65%): LSTM stands out for its ability to capture complex, non-linear relationships and it can learn well from long sequences of data and capture temporal dependencies.
   
![image](https://github.com/53KIbGcAqz0Gokmj/DeYOPOp5UPd8ZajM/assets/143815258/dc8fc152-c51b-4459-8f8d-ff49d3d69e2f)

# Conclusion 

![image](https://github.com/53KIbGcAqz0Gokmj/DeYOPOp5UPd8ZajM/assets/143815258/ac781aa3-b118-442b-8576-569941f95cc7)

