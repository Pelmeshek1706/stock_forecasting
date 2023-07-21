# Stock price forecasting  
#### made by [@pelmeshek1706](https://telegram.me/pelmeshek1706)

In this project, I was involved in predicting the stock chart - whether the price will fall or rise.

**target** will be set to 1 if the closing price of the next trading day is higher than the closing price of the current day, and 0 if it is not. Thus, the 'target' column is created to represent the target variable for the binary classification task based on stock price movement.


 The data was taken from Yahoo and the following libraries were used:
- <code>yfinance</code>
- <code>yahoofinancials</code>
 
 All used libraries:
- <code>numpy</code>
- <code>pandas</code>
- <code>matplotlib</code>
- <code>sklearn</code>
- <code>time</code>


### Results of models for stocks (Google data for the last 10 years was used as an example):

![google_stock](https://github.com/Pelmeshek1706/stock_forecasting/assets/94761102/6f1f6441-159e-4e85-ad9a-9984fffb7cc2)

|№| Model|	Accuracy|	AveragePrecision|	F1|	roc-auc|	Training Time (s)|
|-|------|----------|-------------------|---|--------|---------------------|
|0|	Logistic Regression|	0.519841|	0.528690|	0.612179|	0.509659|	0.311289|
|1|	Decision Tree|	0.521825|	0.535336|	0.530214|	0.522159|	0.247038|
|2|	Random Forest|	0.509921|	0.527250|	0.550091|	0.506818|	2.434921|
|3|	SVC|	0.523810|	0.523810|	0.687500|	0.500000|	0.330786|
|4|	Kneighbours default|	0.537698|	0.542562|	0.569316|	0.535417|	0.006899|
|5|	Gradient Boosting Classifier|	0.519841|	0.530060|	0.593960|	0.512311|	1.136765|
|6|	XGBoost Classifier|	0.523810|	0.534776|	0.558824|	0.521212|	1.595955|
|7|	ADA Boost|	0.529762|	0.535629|	0.597623|	0.522917|	0.209644|
|8|	Naive Bayes	|0.519841|	0.528496|	0.614650|	0.509280|	0.002324|

### Results of models for cryptocurrencies (BTC data for the last 4 years was used as an example)

![btc_stock](https://github.com/Pelmeshek1706/stock_forecasting/assets/94761102/f7453c62-027e-492e-b4fa-ac931210c7cb)

|№| Model|	Accuracy|	AveragePrecision|	F1|	roc-auc|	Training Time (s)|
|-|------|----------|-------------------|---|--------|---------------------|
|0|	Logistic Regression|	0.539007|	0.422209|	0.252874|	0.492901|	0.063593|
|1|	Decision Tree|	0.567376|	0.457429|	0.487395|	0.556481	|0.009441|
|2|	Random Forest|	0.524823|	0.425532|	0.373832|	0.500000|	0.420606|
|3|	SVC|	0.574468|	0.425532|	0.000000|	0.500000|	0.027667|
|4|	Kneighbours default|	0.553191|	0.452084|	0.496000|	0.548457|	0.004485|
|5|	Gradient Boosting Classifier|	0.553191|	0.441135|	0.411215|	0.529012|	0.336344|
|6|	XGBoost Classifier|	0.595745|	0.468652|	0.457143|	0.570370|	0.139248|
|7|	ADA Boost|	0.489362|	0.409026|	0.307692|	0.460494|	0.112277|
|8|	Naive Bayes|	0.439716|	0.428419|	0.590674|	0.505864|	0.002187|

--------------------------------------------------------------------------------------------------------------------------
# Conclusions

*After looking at the results of the models, one can realise that the models are simply guessing whether the price will rise tomorrow or not. This once again confirms that predicting the price of a stock by machine learning is quite difficult. Such algorithms are used in trading bots, and they cost exorbitant amounts of money.*
*It's the same with cryptocurrencies. The price itself is influenced not by the usual exchange indicators, but by many different factors, such as the words of regulators in different countries, the presence of wars/cataclysms or emergencies. It is also worth considering that there is such a story as "Pump" of a certain currency/bond, as it happened recently with GameStop*
