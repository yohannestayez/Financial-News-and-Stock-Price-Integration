## Overview

The project involves analyzing a large corpus of financial news data to discover correlations between news sentiment and stock market movements. The goal is to understand how news sentiment affects stock prices and to identify significant trends and events. The analysis involves a rigorous sentimental and correlation analysis of the financial news dataset.

### Notebooks:
1. Task1: Descriptive Statics, Text analysis (Sentiment analysis & Topic Modeling), Time Series Analysis, Publisher Analysis

2. Task2: Quantitative analysis using TA-Lib and Portfolio analysis
=======
3. Task 3: Correlational analysis


## Project Structure

The repository is structured as follows:

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
│   ├── Analysis.ipynb
│   └── README.md
├── tests/
│   └── __init__.py
└── scripts/
    ├── __init__.py
    └── README.md


## Notebooks

Task1
   - This notebook covers 
    1. Descriptive Statistics:
-  To Obtain basic statistics for textual lengths (like headline length).
-  Count the number of articles per publisher to identify which publishers are most active.
-  Analyze the publication dates to see trends over time, such as increased news frequency on particular days or during specific events.
2. Text Analysis(Sentiment analysis & Topic Modeling):
-  Perform sentiment analysis on headlines to gauge the sentiment (positive, negative, neutral) associated with the news.
-  Use natural language processing to identify common keywords or phrases, potentially extracting topics or significant events (like "FDA approval", "price target", etc.).
3. Time Series Analysis:
-  Analyzes the publication frequency over time.
-  Check for spikes in article publications related to specific market events.
4. Publisher Analysis:
-  Checks which publishers contribute most to the news feed and check the difference in the type of news they report.
-  Identify unique domains to see if certain organizations contribute more frequently.

Task2
-This notebook will cover the quantitative analysis on the historic data using pynance and TA-Lib 

## Setup and Installation

To run the notebooks locally, follow these steps:

1. Clone the repository:
      git clone https://github.com/yohannestayez/Financial-News-and-Stock-Price-Integration.git
   

2. Navigate to the repository:
      cd your-repository-name
   

3. Set up the Python environment:
   - It is recommended to use a virtual environment for the project. Run the following commands to set up and activate it:
          python -m venv venv
     source venv/bin/activate  # On Windows use `venv\Scripts\activate`
     

4. Install the required packages:
   - Install the necessary packages listed in the requirements.txt file (if available):
          pip install -r requirements.txt
     

5. Launch Jupyter Notebook:
   - Start Jupyter Notebook to access and run the notebooks:
          jupyter notebook
     

6. Open the Notebook:
   - Once Jupyter Notebook is launched, open the Task1 notebook to run it interactively.

## Results

The analysis results include:
- Descriptive Statistics
- Text Analysis (Sentiment analysis and Topic modeling)
- Time Series Analysis
- Publisher Analysis

## Contributing

If you'd like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
