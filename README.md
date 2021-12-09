## Homework-10---Time-Series

# Time Series Analysis

In this notebook, I used Time Series analysis to predict the future price of the yen. 

First, I used a Hodrick-Prescott Filter to decompose the yen Settle price into trend and noise. 

Next, I used the ARMA model to forecast returns. (Note: as the ARMA option from statsmodels was depricated, I used the ARIMA option. However, when setting the middle variable to '0', this has the same effect as the ARMA). As the P value was greater than .05, it does not appear that this model will effectively forecast the yen.

Next I used the ARIMA model to forecast Settle price. Similarly to the above, the P value was greater than .05, which indicates this model is not

Finally, I used the GARCH model to forecast volitlity. 

# Regression Analysis

In this notebook, I used Linear Regression Forecasting to predict the future price of the yen. I prepared the data, fit the model, made predections using the testing data, and then examined the out-of-sample and in-sample performance. In this case the out-of-sample data performed better. 