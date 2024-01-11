# Jupyter Notebook README


# Jasmine, Jordan, Sean, Vineet
## Each of us used our own branch. So contributer stats are not accurate for the default branch.

## Overview
This Jupyter notebook is a comprehensive analysis of the correlation between Google trends and stock data, specifically focusing on Nike (NKE) and related consumer search terms. The analysis highlights trends in November and December and introduces a trading algorithm that outperforms the S&P 500. 

## Seasonal Advertising Strategy
In addition to the core analysis, this notebook also explores how companies like Nike, Pandora, Airbnb, and Carnival Cruise Lines can leverage Google Trends data to optimize their advertising strategies seasonally. This branch of the analysis focuses on identifying specific months and seasons where consumer interest in products peaks, allowing for targeted advertising efforts. By understanding these patterns, companies can allocate their marketing resources more effectively, ensuring that they are advertising their products during periods of high consumer interest, thereby potentially increasing sales and market presence.

## Dependencies
- Prophet: For time series forecasting.
- yfinance: To fetch financial data.

## Key Functions
1. **`clean_dataframes(dfs_list)`**: Cleans given list of dataframes by dropping specific rows.

2. **`merge_and_plot_dfs(df_list, merge_on='Month', plot=True)`**: Merges multiple dataframes on a specified column and optionally plots the merged data.

3. **`get_stock_data(ticker_symbols, start_date, end_date)`**: Fetches stock data for given ticker symbols over a specified period.

4. **`remove_open(list_of_stocks)`**: Removes 'Open' column from stock dataframes.

5. **`logistic_forecast(df)`**: Performs a logistic forecast on a dataframe using the Prophet model.

6. **`df_forecast(df_list)`**: Applies forecasting on a list of dataframes and stores the results.

7. **`calc_prof(df)`**: Calculates profit based on buy and sell conditions in the dataset.

8. **`get_good_corr(split_corr_dfs, stock_dfs, threshold)`**: Identifies dataframes with correlation values above a certain threshold.

## Analysis Flow
1. Import Libraries: pandas, requests, json, datetime, matplotlib, yfinance, IPython.display.
2. Define utility functions for data cleaning, merging, and plotting.
3. Import and clean Google Trends data related to Nike.
4. Define Nike (NKE) stock ticker and fetch corresponding stock data.
5. Merge and analyze stock and Google Trends data, looking for correlation and trends.
6. Apply Prophet models for forecasting trends and analyzing future patterns.
7. Identify profitable trading strategies based on the correlation between stock performance and consumer interest over time.

## Highlights
- The analysis identifies key months (November and December) where consumer search trends correlate strongly with Nike's stock performance.
- A trading algorithm based on this correlation is shown to outperform the S&P 500, suggesting a viable strategy for stock trading based on consumer trends.

## Usage
To use this notebook, ensure all dependencies are installed, and run each cell sequentially. The notebook is structured to guide the user through the data import, cleaning, analysis, and forecasting steps, culminating in insights into the relationship between consumer trends and stock performance.
