
# Portfolio Analysis and TA-Lib Financial Metrics

## Overview
This project involves analyzing historical stock data to perform portfolio analysis and calculate various financial metrics using TA-Lib. The goal is to optimize a portfolio of stocks, evaluate its performance, and visualize the results.

## Folder Structure
Analysis3.ipynb : Script to perform portfolio analysis.
Analysis2.ipynb : Script to calculate financial metrics using TA-Lib.

## Dependencies
pandas: For data manipulation and analysis.
numpy: For numerical operations.
matplotlib: For plotting and visualization.
TA-Lib: For technical analysis indicators.

## Load Historical Data

Reads historical stock data from CSV files.
Filters data for the year 2020.
## Calculate Daily Returns
Computes daily returns from adjusted close prices.

## Simulate Portfolios
- Generates random portfolios by assigning random weights to each stock.
- Calculates expected return, risk (volatility), and Sharpe Ratio for each portfolio.

## Optimization and Results
- This script calculates various financial metrics using TA-Lib
- Identifies the portfolio with the highest Sharpe Ratio.
- Saves portfolio metrics, including weights, return, risk, and Sharpe Ratio, to a CSV file.
- Visualizes the Efficient Frontier with a color gradient representing Sharpe Ratios.
- portfolio_analysis_2020.csv: Contains the portfolio analysis results including portfolio weights, return, risk, and Sharpe Ratio.
- A plot visualizing the Efficient Frontier with Sharpe Ratios.


## Load Historical Data
- Reads historical stock data from CSV files.
- Apply TA-Lib Indicators:

- Moving Averages: Calculates Simple Moving Averages (SMA) and Exponential Moving Averages (EMA).
- Relative Strength Index (RSI): Measures momentum and potential overbought/oversold conditions.
- Moving Average Convergence Divergence (MACD): Analyzes trend and momentum.



## Notes
Ensure that the paths to the data files in the scripts are correctly specified.
Adjust the parameters of the TA-Lib functions as needed to fit your specific analysis requirements.
Review the portfolio_analysis.py script to modify the number of portfolios simulated or to include additional metrics.

## Contributing
If you have suggestions or improvements for this project, feel free to contribute by submitting a pull request or opening an issue.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.