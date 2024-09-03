# Financial News and Stock Price Integration Analysis

## Overview

This project focuses on analyzing a large corpus of financial news data to uncover correlations between news sentiment and stock market movements. The goal is to understand how news sentiment affects stock prices, identify significant trends and events, and use technical analysis for quantitative insights. The analysis is split into multiple tasks covering descriptive statistics, sentiment analysis, time series analysis, publisher analysis, and correlation analysis between news sentiment and stock performance.

## Project Structure

The repository is structured as follows:

```
├── .vscode/
│   └── settings.json
├── .github/
│   └── workflows/
│       └── unittests.yml
├── .gitignore
├── requirements.txt
├── README.md
├── src/
│   └── __init__.py
├── notebooks/
│   ├── __init__.py
│   ├── Analysis1.ipynb
│   ├── Analysis2.ipynb
│   ├── Analysis3.ipynb
│   ├── Analysis4.ipynb
│   └── README.md
├── tests/
│   └── __init__.py
└── scripts/
    ├── __init__.py
    └── README.md
```

## Notebooks

### Analysis1

This notebook covers:

1. **Descriptive Statistics:**
   - Obtain basic statistics for textual lengths (like headline length).
   - Count the number of articles per publisher to identify the most active publishers.
   - Analyze the publication dates to identify trends over time, such as increased news frequency on particular days or during specific events.

2. **Text Analysis (Sentiment Analysis & Topic Modeling):**
   - Perform sentiment analysis on headlines to gauge the sentiment (positive, negative, neutral) associated with the news.
   - Use natural language processing (NLP) to identify common keywords or phrases, potentially extracting topics or significant events (like "FDA approval," "price target," etc.).

3. **Time Series Analysis:**
   - Analyze publication frequency over time.
   - Check for spikes in article publications related to specific market events.
   - Examine the alignment of news data with stock price data by normalizing timestamps.

4. **Publisher Analysis:**
   - Identify which publishers contribute most to the news feed and examine the differences in the type of news they report.
   - Identify unique domains to see if certain organizations contribute more frequently.

### Analysis2

This notebook covers:

- **Quantitative Analysis Using TA-Lib:**
   - Calculation of financial metrics such as EMA (Exponential Moving Average), SMA (Simple Moving Average), MA (Moving Average), MACD (Moving Average Convergence Divergence), volatility, and RSI (Relative Strength Index).
   - Visualization of these indicators to better understand their impact on stock prices.

### Analysis3

This notebook covers:

- **Portfolio Analysis:**
   - Simulation of portfolio optimization based on historical stock data.
   - Calculation and visualization of portfolio performance metrics including expected returns, risk (volatility), and Sharpe ratio.
   - Evaluation of portfolio weight distributions for optimal performance.

### Analysis4

This notebook covers:

- **Correlation Analysis:**
   - Establishing statistical correlations between the sentiment derived from news articles and the corresponding stock price movements.
   - Tracking stock price changes around the publication date of news articles and analyzing the impact of news sentiment on stock performance.
   - Performing lagged correlation analysis to assess the impact of news sentiment over multiple days.
   - Visual representation of correlation results to highlight key relationships.

## Setup and Installation

To run the notebooks locally, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yohannestayez/Financial-News-and-Stock-Price-Integration.git
   ```

2. **Navigate to the repository:**
   ```bash
   cd Financial-News-and-Stock-Price-Integration
   ```

3. **Set up the Python environment:**
   - It is recommended to use a virtual environment for the project. Run the following commands to set up and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   ```

4. **Install the required packages:**
   - Install the necessary packages listed in the requirements.txt file:
   ```bash
   pip install -r requirements.txt
   ```

5. **Launch Jupyter Notebook:**
   - Start Jupyter Notebook to access and run the notebooks:
   ```bash
   jupyter notebook
   ```

6. **Open the Notebook:**
   - Once Jupyter Notebook is launched, open the respective notebook (e.g., `Analysis1.ipynb`) to run it interactively.

## Results

The analysis results include:

- **Descriptive Statistics:** Overview of headline lengths, article counts per publisher, and publication trends.
- **Text Analysis:** Sentiment analysis results and key topics or phrases extracted from headlines.
- **Time Series Analysis:** Insights into publication frequency trends and alignment with stock price data.
- **Publisher Analysis:** Contributions of different publishers and their focus areas.
- **Quantitative Analysis:** Technical indicators calculated using TA-Lib and their impact on stock prices.
- **Portfolio Analysis:** Optimized portfolio metrics and visualizations.
- **Correlation Analysis:** Statistical correlations between news sentiment and stock price movements, including lagged effects.

## Contributing

If you'd like to contribute to this project, please fork the repository and submit a pull request. Contributions related to improving the analysis, adding new financial metrics, or enhancing visualizations are welcome.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

