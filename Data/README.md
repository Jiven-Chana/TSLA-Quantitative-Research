# Data CSV Folder #

This folder contains all the normalized data for various assets and metrics used throughout the repository, including:
	•	TSLA (Tesla)
	•	NDX (Nasdaq 100 Index)
	•	XLY (Consumer Discretionary Select Sector SPDR)
	•	DRIV (Global X Autonomous & Electric Vehicles ETF)
	•	LIT (Global X Lithium & Battery Tech ETF)
	•	Volatility Data
	•	VWAP Data

## File Contents ##

Each CSV file daily observations of:
	•	Date
	•	Open, High, Low, Close prices
  • Volumes, dividends
 
Each normalised CSV file includes daily observations of:
	•	Date (often used as the index)
	•	Open, High, Low, Close prices (normalized)
	•	Volatility (varies by dataset; e.g., standard deviation, ATR, or custom measure)
	•	VWAP (Volume Weighted Average Price)
 
## Notes & Disclaimers ##
1.	Data Sources: The CSV files are derived or downloaded from yahoo finance API. Be aware of potential licensing or usage restrictions if you plan to redistribute.
2.	Normalization: Values here are scaled or normalized relative to some baseline (e.g., min-max scaling)
3.	Accuracy: While every effort has been made to ensure data quality, no warranty is given as to its completeness or accuracy. Use at your own risk.
4.	Contribution: If you find discrepancies or wish to add more datasets, feel free to open a pull request or file an issue in this repository.
