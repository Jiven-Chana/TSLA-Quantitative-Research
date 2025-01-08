# Data Processing Directory

This folder contains Jupyter notebooks that are used for processing and analyzing financial data. The notebooks are designed to manipulate and prepare datasets stored in another directory, typically involving normalization, scaling, and various transformations required for subsequent analysis and modeling.

## Overview

The notebooks in this directory perform a range of data processing tasks on several financial instruments and indices including:

- **TSLA (Tesla Inc.)**
- **NDX (Nasdaq 100 Index)**
- **DRIV (Global X Autonomous & Electric Vehicles ETF)**
- **XLY (Consumer Discretionary Select Sector SPDR Fund)**
- **LIT (Global X Lithium & Battery Tech ETF)**

These notebooks include operations such as:

- **Normalization of financial data** to ensure consistency in scale across different datasets.
- **Calculation of Volatility** using historical price data.
- **VWAP computation** for each stock and index to reflect the average trading price across the day, weighted by volume.
- **Composite index creation** to blend various indices based on specified weights.

## Usage Instructions

1. **Set Up**: Ensure you have a Python environment capable of running Jupyter notebooks, with necessary libraries such as `pandas`, `numpy`, `matplotlib`, `sklearn`, and others installed.
   
2. **Data Paths**: Adjust the data file paths in each notebook to match the location where the CSV files are stored:
   ```python
   pd.read_csv('<path_to_your_data_directory>/TSLA_data1.csv', index_col='Date', parse_dates=True)
3.	Execution: Run the notebooks in a Jupyter environment to process and analyze the data. Each notebook contains detailed comments explaining each step of the process.

## Contributing ##
•	Improvements: If you have suggestions for improving the data processing or analysis, please feel free to fork this repository and submit your changes via a pull request.
•	Issues: For any problems or bugs in the notebooks, please open an issue in this repository detailing the issue and any suggested fixes.

## Disclaimer ##

The data processing scripts in this directory are for educational and research purposes only. Users are encouraged to verify the appropriateness of the techniques used here for their specific data needs and contexts.
