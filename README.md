# Background #

This is my first time working with python, Jypter Notebooks, and Kaggle but I'm going to continue to develope this program in the background and hopefully finish it.

More information about the programs purpose can be found here: <https://github.com/uiuc-quant/assessments/blob/ml-correlation-model/ml-correlation-model/README.md>

# Appraoch Method #


**1. Complie the monthly average price of the S&P500, Foex Market, and any other markets such as the DJIA, NASDAQ, and others.**
*(Since we are dealing with longer time periods monthly averages make more sense over hourly or daily.)*


### 2. Compare the Forex dataset to an equity market dataset by gradually shifting the datasets in a +-6 month time frame. ###
*(+-6 months because after that time period there may be too much external noise unaccounted for or the market may repeat it's standard yearly lows and highs if it were compared on a +-12 month scale)*


### 3. Compare the price difference of the Forex Market and an equity market on a monthly basis gradually shifting the timeframe on one of the datasets. ###


### 4. Use the shifted time frame that produced the lowest consistent difference (Direct Correlation) or that produced the largest consistent difference (Inverse Corrleation). ###
*(May be possible to incorporate standard deviation to find the timeframe with the least average monthly variaiton in difference between the markets.)*


### 5. Once a relationship between the markets is found use multiple regression to create a machine learning model. ###



### 6. Train the model with 80% of the data, and test with the remaining 20%. ###


### 7. If all fails: Begin exploring decsion trees and incorporating them into the model. ###


# Program Status #

The program is currently able to download datasets from Kaggle and unzip them. It can compile hourly Euro/USD Forex data into monthly averages and store them in a .csv file. It can also graph the monthly average. The next step is to repeat the unzip and averaging process for each equity market to be analyzed. Then the data set shifitng mechanism needs to be implemented and the subsequenclty the difference calculator and logger to find the timeframe. Finally, the multiple regression and model training would be implemented assuming everyhting works.

Currently, only the Euro/USD are analyzed but it may be interesting to compare the USD against the Peso, Yen, or Pound Sterling as well. I will also look into adding more advanced graphing features along with interactivity for the user.
