# Crypto_Abritrage_Application

This program is to develop a **Python** application (using Pandas) that will perform calculations to determine whether Cryptocurrency arbitrage opportunities exist for Bitcoin on two exchanges, Bitstamp and Coinbase. To perform this calculations, historical data is provided in the ```bitstamp.csv and coinbase.csv``` files. 

User can select specific periods of time (a month) and dates (15th of every month) for Time Series Analysis. Once these parameters are selected, the application performs calculations, compares the pricing of Bitcoin on both exchanges and calculates any abritrage opportunities. Box and Plot charts are also utilized as visuals to better understand the data and the analystics.

---

## Technologies

This application is developed on the **Python** *3.7.11 version*. Jupyter Lab Notebook is used for running the program. It incorportates the following required dependancies to run. These dependancies include the following Imports:

1. **Pandas** = To import functions needed to program application
2. **Pathlib** = To load and save files from and to paths.
3. **%matplotlib inline** = To perform analytical calculations.


---

## Installation Guide

The following PIP installation must be performed before running the program. It includes:

```pip install pathlib```
```install Jupyter Lab```

---

## Usage
This section should include screenshots, code blocks, or animations explaining how to use this program.

**Data Collection and Preparation

In preparing these data collections, Bitstamp.cvs and Coinbase.csv dataframes need to be imported and read into the program. To confirm this, review the first 5 rows or last 5 rows of the dataframes. Once this is done, the next step is to prepare and to clean the dataframes for statistical analysis. For instance, in the "Close" columns of the dataframes, there are dolloar signs in front of the numbers; these need to be removed for the program to execute it's calculations. Also, NaN values must be removed and the datatypes must be set to float64.


**Analyzing the Data and Calculating the Arbitrage Profitability

To analyze the data, select 'Timestamp' and 'Close' columns as the specific areas of focus. The Close column is analyzed, as it is the closing price for BTC on each exchange.  

Then, review the 'Summary Statistics' and plot the data on charts for all data. Here, both exchanges are plotted for BTC prices; then, the plots are overlayed to determine any difference in prices visually.

To focus on specific dates (areas of interest), select the day to analyze. For example, the 15th of each month is selected. These three date will be compared to each other to measure: arbitrage spread, spread returns and profitability. 

Now, to further zoom in on the analysis, let's look at profits per trade and calculate the trades that exceeded the 1 percent transaction fee/cost. This will identify the opportunities to make a 'net' profit trading BTC on 2 different exchanges.

As User processes the program, verification of data and information need to be performed to validate its accuracy. To review the program code results, .describe(), .head()/.tail() are used for validation. Once done, then plotting box charts and line graphs provide a visual to see the results.

**Reporting

The results from this financial analysis conclude that opportunities for profitable BTC arbitrage between 2 exchanges is very slim to non existant. 

Let's review the findings from this example:

1st. The dataframes and timeframes are identified; from the CSV files in the resource folder, the timeframe is the Q1 of 2018. Each data from holds approximately 129,000 rows and 7 columns. The Close BTC price on 01-01-2018 is $13646.46 on Bitstamp and $13608.49 on Coinbase. And the Close BTC price on 03-31-2018 is $6928.01 on Bitstamp and $6934.0 on Coinbase. Therefore, over this period of time, the price of BTC was declined significantly; a contributing factor to the non existant profitable arbitrage opportunities.

Here, monthly and one daily analysis is performed; targeted areas of focus are the 15th of each month (Jan, Feb and Mar). Also, 

2nd. For each of the 3 dates, calculations are performed for:
   the *arbitrage spread* between Bitstamp and Coinbase exchanges,
   the *spread returns*,
   the *potential profit, in dollars, per trade* 
   the *potential arbitrage profits* for each 15th of the month, and
   the *cumulative sum* for each of the 3 dataframes.

3rd. Summary statistics examined.

4th. Visualizations: Plots
    Box Plots
    

---

## Contributors

Contributor: John Batarse  

Email: jbatarse@hotmail.com

LinkedIn: [Find me on LinkedIn](<https://www.linkedin.com/in/john-a-batarse-760a26116/>)

---

## License

Trilogy Education, LLC / UC Berkeley