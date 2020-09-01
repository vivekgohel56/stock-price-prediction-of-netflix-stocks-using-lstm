# stock-price-prediction-of-netflix-stocks-using-lstm

stock market analysis is divided into two parts – Fundamental Analysis and Technical Analysis.

Fundamental Analysis involves analyzing the company’s future profitability on the basis of its current business environment and financial performance.

Technical Analysis, on the other hand, includes reading the charts and using statistical figures to identify the trends in the stock market.
 our focus will be on the technical analysis part.
 
Stock traders mainly use three indicators for prediction: OHLC average (average of Open, High, Low and Closing Prices), HLC average (average of High, Low, and Closing Prices), and Closing price, In this project, the OHLC average has been used.
All values have been normalized between 0 and 1.

The predicted closing price for each day will be the average of a set of previously observed values. Instead of using the simple average, we will be using the moving average technique which uses the latest set of values for each prediction. In other words, for each subsequent step, the predicted values are taken into consideration while removing the oldest observed value from the set.

Two sequential LSTM layers and in between dropout of rate 0.25 have been stacked together and one dense layer is used to build the RNN model using Keras deep learning library. Since this is a regression task, 'linear' activation has been used in the final layer.

Refrence:- https://www.analyticsvidhya.com/blog/2018/10/predicting-stock-price-machine-learningnd-deep-learning-techniques-python/?#
https://github.com/NourozR/Stock-Price-Prediction-LSTM

Results:-
![alt text](https://github.com/vivekgohel56/stock-price-prediction-of-netflix-stocks-using-lstm/blob/master/diff_btwn_diff_avgs.png?raw=true, "Diff_averages")
![alt text](https://github.com/vivekgohel56/stock-price-prediction-of-netflix-stocks-using-lstm/blob/master/graph_of_predicted_data.png?raw=true, "Graph of valid/test data")
