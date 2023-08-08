# Climate Change and Seasonality Analysis README
Final Project located in files:

- Final-Climate-Seasonality-Analysis.ipynb
- climate_seasonality_analysis.ipynb
- Demo_Graph.ipynb

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

## Features

### Downloading Ticker Data
The script downloads the data for selected ticker symbols representing ETFs from Yahoo Finance using YFinance API and calculates the weekly returns for each ETF.

### Sector Analysis and Performance Statistics
The script generates plots for several performance metrics of the ETFs:
- ! [Closing price plotted for the period 2008-2023](Resources/PriceperShare_SectorETFs.png)
- ! [Cumulative Returns](Resources/Sector_Cumulative_Returns.png)
- ! [Sharpe Ratio](Resources/Sharpe_by_Sector.png)
- ! [Riskiness (Standard Deviation of Weekly Returns)](Resources/StDev_by_Sector.png)
- ! [Correlation of Weekly Returns](Resources/Sector_Correlations.png)
- ! [Static Betas for Period 2008-2023](Resources/Static_Sector_Betas.png)
- ! [52-Week Rolling Betas from 2008-2023](Resources/Rolling_Sector_Betas.png)

### Seasonality Analysis
This section analyzes the seasonality in the ETF returns. It fetches daily data for each ticker and assigns a season based on the month of the year. It then calculates the average seasonal returns for each ETF.

- ! [ETF Variance by Season](Resources/sideways_Consolidation.png)
- ! [Seasonal Adjustments - Market Consolidation](Resources/sideways_Consolidation.png)
- ! [Seasonal Adjustments - Bull Market](Resources/bull_market_conditions.png)
- ! [Monthly Returns Box Plot](Resources/boxplot.png)
- ! [Seasonality & 20MA of SPY](Resources/download.png)

## Findings and Conclusions

There do appear to be seasonal effects in the stock market. Over the 15 years in the dataset, this effect is most pronounced in Winter, or Q4. ETFs experienced greater volatility in these Winter months, and not so much in the Spring.

In terms of climate, the data suggest that increasing surface temperature was correlated with lower returns, while a decrease in surface temperature was associated with better returns. More research needs to be done over a greater period of time to determine to what extent climate has a causal impact on returns.

## Next Steps

- Adding different factors into our analysis - macro economic factors, inflation, interest rates, natural disasters, geopolitical climate
- Diving deeper into what extent climate change effects the performance of different industry stock prices
- Going deeper and broader with seasonality/trends analysis - running more tests on ETF’s, etc.
- Drawing conclusions from our data that will help us facilitate our investment strategy
- For the climate change analysis, we want to dive deeper and add in other variables, such as natural disasters, and explore further risk ratios to see if there are any trends.
