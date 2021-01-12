# time_series_regress

## Time Series Analysis ##

### At First Glance, our Yen to USD Settle Prices Appear to be Quite Volatile ###

![](https://github.com/alexgwise/time_series_regress/blob/main/pictures/yen_graph.PNG)

### The Amount of Noise is Also Quite High ###

![](https://github.com/alexgwise/time_series_regress/blob/main/pictures/noise.PNG)

### The ARMA Model ###

The ARMA model was NOT able to generate statistically significant p-values and therefore
does not appear to be a good model. There are likely factors contributing to the 
volatility in the Yen to USD price that we are not capturing.

![](https://github.com/alexgwise/time_series_regress/blob/main/pictures/ARMA%20p-value.PNG)

### The ARIMA Model ###

Based on the very high p-values, we cannot reject the null hypothesis.
Our model does not appear to be statistically significant. The additional AR's did not
make for a better model, and our AIC and BIC scores became much worse compared to the 
ARMA model based on the same data.

![](https://github.com/alexgwise/time_series_regress/blob/main/pictures/ARIMA.PNG)

### GARCH Volatility ###

Finally, the GARCH model would indicate the volatity is increasing.
I would not feel confident in using these models to trade, based on the volatility, and poor p-values which do not reject the null hypothesis.

![](https://github.com/alexgwise/time_series_regress/blob/main/pictures/GARCH%20Volatility.PNG)
