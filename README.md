# Time_Series

For this assignment, I used both time series models and a linear regression model forecast movements in the exchange rate between the Japanese Yen against the Canadian Dollar.

Using 29 years of CAD-JPY exchange rate data (from January 1990 through June 2020) as an input, I ran the following models to forecast on various aspects of the Yen over the next 5 trading days:

ARMA Model - to predict returns
ARIMA Model - to predict price
GARCH Model - to predict volatility

Based on these results derived from these models, I predicted that returns on the Yen should decrease over time, and its value should fall vs. the Canadian dollar, and volatility should rise. As such, I can draw the conclusion that it would not be a good idea to buy Yen at this time. However, due to a high p-value for each of these models, I cannot fully rely on these forecasts.

Following this analysis, I used the same dataset to construct a linear regression model aimed at forecasting returns for the yen. I trained the model on returns data from 1990 to 2020. Once trained, I fed this model both the in-sample data used to train the model and out-of-sample from 2020 to forecast historical returns. When comparing the outputs of the in-sample and out-of-sample applications of this model, I found that the root mean squared error for the out-of-sample application was actually lower than for the in-sample application, giving me confidence that this model could be used to make somewhat accurate predictions on data it is not familiar with.
