
## Overview

This project involves analyzing historical stock data to perform portfolio analysis and calculate various financial metrics using TA-Lib. Additionally, it includes a comprehensive correlation analysis to understand the relationship between news sentiment and stock price movements. The objective is to optimize a portfolio of stocks, evaluate its performance, analyze correlations, and visualize the results using both technical analysis and statistical methods.

## Folder Structure

```
├── Analysis1.ipynb : Scripts to perform descriptive statistics, sentiment analysis, time series analysis, and publisher analysis.
├── Analysis2.ipynb : Script to calculate financial metrics using TA-Lib, including Moving Averages, RSI, and MACD.
├── Analysis3.ipynb : Script to perform portfolio analysis, including simulation of portfolios and evaluation of their performance metrics.
├── Analysis4.ipynb : Scripts to perform correlation analysis between news sentiment and stock price movements.
```

## Dependencies

- **pandas**: For data manipulation and analysis.
- **numpy**: For numerical operations.
- **matplotlib**: For plotting and visualization.
- **TA-Lib**: For technical analysis of financial data.
- **seaborn**: For enhanced data visualization.
- **nltk**: For natural language processing tasks, particularly in sentiment analysis.
- **glob**: For file path management.
- **vadersentiment**: For sentiment analysis of text data.

## Analysis Workflow

### Load Historical Data

- **Data Sources**: The scripts load historical stock data from CSV files. Ensure the paths to the data files are correctly specified in the notebooks.
- **Filtering**: Data is filtered to focus on the year 2020, aligning the analysis with specific timeframes of interest.

### Calculate Daily Returns

- **Daily Returns**: The scripts compute daily returns from adjusted close prices, which form the basis for subsequent portfolio analysis.

### Simulate Portfolios

- **Portfolio Generation**: The analysis simulates random portfolios by assigning random weights to each stock. This allows for exploration of a wide variety of potential portfolio combinations.
- **Performance Metrics**: For each portfolio, expected return, risk (volatility), and the Sharpe Ratio are calculated. These metrics are crucial for evaluating portfolio performance.

### Optimization and Results

- **TA-Lib Financial Metrics**: This step involves the calculation of various technical indicators using TA-Lib:
  - **Moving Averages**: Both Simple Moving Averages (SMA) and Exponential Moving Averages (EMA) are calculated.
  - **Relative Strength Index (RSI)**: Used to measure momentum and identify potential overbought/oversold conditions.
  - **Moving Average Convergence Divergence (MACD)**: Analyzes trend and momentum, providing insights into the stock's movement.

- **Portfolio Optimization**: The portfolio with the highest Sharpe Ratio is identified, representing the optimal balance between risk and return.

- **Output**:
  - **portfolio_analysis_2020.csv**: Contains the portfolio analysis results, including portfolio weights, return, risk, and Sharpe Ratio.
  - **Efficient Frontier Plot**: A visual representation of the Efficient Frontier, with a color gradient indicating the Sharpe Ratios of the simulated portfolios.

### Correlation Analysis

- **Analysis4.ipynb**: This notebook focuses on establishing statistical correlations between the sentiment derived from news articles and the corresponding stock price movements. The analysis tracks stock price changes around the publication dates of news articles and evaluates the impact of news sentiment on stock performance.
  - **Correlation Metrics**: The correlation coefficients between sentiment scores and stock returns are calculated.
  - **Visualization**: Correlation heatmaps and scatter plots are generated to visually represent the relationships between news sentiment and stock price movements.
  - **Insights**: This analysis helps identify significant patterns and relationships, providing insights into how market sentiment influences stock prices.

## Notes

- **Data Paths**: Ensure that the paths to the data files in the scripts are correctly specified before running the analysis.
- **TA-Lib Parameters**: The parameters of the TA-Lib functions can be adjusted as needed to fit your specific analysis requirements.
- **Customization**: The portfolio simulation process can be customized by modifying the number of portfolios generated or by including additional metrics in the `Analysis3.ipynb` notebook.

## Contributing

If you have suggestions or improvements for this project, feel free to contribute by submitting a pull request or opening an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

