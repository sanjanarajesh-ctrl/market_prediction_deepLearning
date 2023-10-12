The project's purpose was to predict stock prices using LTSMs and RNNs. I used the daily price history of NASDAQ stocks for the past 20 years from AlphaVantage. The data included open, high, low, close, and volume of trades for each day, since 1999. 

A vital feature of this model is a complex network structure with two inputs with distinctive layer types in each branch. It has 50 LTSM cells in the first layer, a dropout layer to prevent overfitting, and a few dense layers.  A highlight of this network the linear output activation that allows the model to accurately tune its penultimate weights. 

I also created a simple bot to make buy/sell decisions for the day. The bot predicts the opening value of the stock for the next day, and if it is beyond a threshold amount, it buys the stock. If it is below another threshold amount, it sells the stock.
