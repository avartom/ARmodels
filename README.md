# AR Models
New methods of autoregressive models to predict time series. First, we partition the data into N sets and then apply an AR/ARMA/ARIMA models separately to each dataset in the partition. Then, we use the remaining N-1 datasets in the partition to predict using the above time series forecasting models. These predictions will form the feature space containing N featurs and the target variable which is the future value of the times series. Thus we will turn a times series forecasting model into a non-AR problem. 

There is also an analogue of ARMA version that computes the mean of the different autoregressive models (more on this later). Next, we introduce some kind of averaging of the different AR's and ARMAs to prevent overfitting. 
