# Stock-Predictor
Simple Python Project that predicts the next day closing price of the securities on the SP500 Index

# Problem to be solved
Investing in index funds and ETFs that mimic the benchmark are only able to provide “average” returns. This is the very nature of their design, they exist to shield investors from risks, excessive fees and the complexity of picking stocks. Their obvious downside is the potential gains that are left on the table to investors who are willing to risk their dollars in pursuit of higher returns. I recognize there is an opportunity to use AI technologies to predict the closing price of stocks and potentially return results that are greater than the benchmark. 

# Desired Outcome
Invest (gamble*) in the stock market with the intention of finding stocks that will outperform the index so that I can realize gains that are higher than the average. 

# Day trading method:
I recognize that there is an infinite number of different approaches that can be used in Day Trading of stocks and commodities. I don’t suggest that I have a special ability to beat the market, nor do I consider myself literate in this practice. I’ve developed an elementary algorithm that allows me to demonstrate the ability for ML and DL Models to solve this task. 

I will take a collection of different stocks and feed them into the model for a prediction of tomorrow’s closing price. Then, using MatPlotLib, I will calculate the percent change from open to close. For the top three stocks, I will purchase an equal amount of those at open and then sell them at close. 

# Methods to employ
* We will develop different models and then use Arize.AI to benchmark their performance against each other. The number of models and their design is yet to be determined. Here is a suggested list that we will iterate through. 
* A simple RNN using the last 30 days of closing price for stocks. 
* An improved RNN using the last 30 days of closing price, plus some additional features for the model. 
* A simple ML regression model using multiple features. Developed and designed using Microsoft ML Studio. 

# Sourcing the data

# Measuring Performance
MAPE: I will measure the predicted values and then their actuals at the close of the day. I will be able to calculate mean absolute percent error for all stocks that we predicted because we will know actual values within 24 hours. 
Performance against the benchmark. I’ll be able to track the total return of my portfolio as compared to just investing the traditional and safe way of parking your capital in an ETF. I’ll choose an ETF as the benchmark because it allows for day trading, unlike an Index Fund. 

***

# High level components of the system

# Data gathering
* From a CSV list of stock symbols, the system will query Yahoo Finance via the YFinance Python Library.
* Data about each symbol will be loaded into a dataframe and then persisted into a CSV file with a name of [date+stockinformation.csv]

# Model Training
* Given today’s date, go open the file with today’s stock information. 
* Trail a RNN model 
* Deploy this model

# Model Prediction
* Open the CSV file that contains all of the stocks. 

# Model Benchmarking
* At the close of each day get the closing values 


