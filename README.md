# Sector Analysis README

## Description
This Python program performs sector analysis on a set of Exchange Traded Funds (ETFs) that represent various sectors of the economy. It extracts stock market data using the Yahoo Finance (YFinance) library and performs analysis on several aspects like weekly returns, Sharpe Ratio, Risk, Correlation, Beta, Rolling Beta, and Seasonality. This analysis is primarily based on the time period from 2008 to 2023. 

The tool provides interactive charts and plots using the hvplot library for visualizing various metrics.

## Libraries Used
- pandas
- pandas_datareader
- yfinance
- hvplot
- numpy
- pathlib
- datetime

## Features

### Downloading Ticker Data
The script downloads the data for selected ticker symbols representing ETFs from Yahoo Finance using YFinance API and calculates the weekly returns for each ETF.

### Sector Analysis and Performance Statistics
The script generates plots for several performance metrics of the ETFs:
- Closing price plotted for the period 2008-2023.
- Cumulative Returns
- Sharpe Ratio
- Riskiness (Standard Deviation of Weekly Returns)
- Correlation of Weekly Returns
- Static Betas for Period 2008-2023
- 52-Week Rolling Betas from 2008-2023

### Seasonality Analysis
This section analyzes the seasonality in the ETF returns. It fetches daily data for each ticker and assigns a season based on the month of the year. It then calculates the average seasonal returns for each ETF.

### Seasonal Decomposition
Lastly, the script performs a seasonal decomposition analysis of the S&P 500 ETF (SPY).

## Requirements
To use this script, you will need to have Python installed along with the libraries mentioned above. 

## How to Use
1. Ensure all dependencies are installed.
2. Clone the repository.
3. Run the script in a Jupyter Notebook environment.
4. Modify the tickers list to add or remove ETFs for analysis.
5. Adjust the start and end date variables in the Seasonality Analysis section if a different time range is needed.

## Note
The data downloaded from YFinance is dependent on their API which may change, and the data availability can be limited or delayed based on their rules. Make sure to check their documentation for any updates or limitations.

This script does not provide financial advice. It's a tool for analysis and understanding sector performance. Please consult with a financial advisor before making investment decisions.
