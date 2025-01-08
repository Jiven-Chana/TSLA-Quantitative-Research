# Financial Data Analysis with Kalman Filter

This repository contains a Python script that demonstrates the application of a Kalman Filter to analyze the dynamic beta and alpha between the stock returns of Tesla (TSLA) and the Nasdaq 100 index (NDXL). The script performs a detailed time series analysis, visualizes the relationship dynamics, and calculates statistical metrics.

## Description

The script performs the following operations:

1. **Data Loading**: Loads normalized closing price data for TSLA and NDXL from CSV files.
2. **Data Alignment**: Aligns both datasets by date and calculates the daily returns.
3. **Kalman Filter Initialization and Application**:
   - Initializes a Kalman Filter to estimate the dynamic states (beta and alpha) of the returns data.
   - Uses the returns to calculate and update the estimates continuously.
4. **Visualization**:
   - Plots the rolling beta and alpha over time to visualize their changes.
   - Creates a scatter plot with regression lines to illustrate the relationship between the returns of TSLA and NDXL.
5. **Analysis Output**:
   - Displays the shape of the data frame, date range, and the calculated state means.
   - Outputs additional regression analysis with an Ordinary Least Squares (OLS) line for comparison.

## File Structure

- `TSLA_Normalised_OHLC_VWAP_VOL.csv`: Contains the normalized open, high, low, close, volume, and VWAP data for TSLA.
- `NDXL_Normalised_OHLC_VWAP_VOL.csv`: Contains the normalized open, high, low, close, volume, and VWAP data for NDXL.

## Usage

Ensure the following libraries are installed before running the script:

- `numpy`
- `pandas`
- `matplotlib`
- `pykalman`

To run the script, navigate to the script's directory and execute it in a Python environment:

```bash
python kalman_filter_analysis.py
```

## Visualizations

The script generates two main visualizations:
	1.	Rolling Beta and Alpha Plot: Shows how the relationships between TSLA and NDXL evolve over time.
	2.	Scatter Plot with Regression Lines: Highlights the correlation between the returns and overlays a linear regression model to benchmark against the Kalman Filter’s output.

## Configuration

Modify the paths to the CSV files within the script if your files are located in a different directory:

```python
tsla_data = pd.read_csv('<path_to_data>/TSLA_Normalised_OHLC_VWAP_VOL.csv', index_col='Date', parse_dates=True)
ndxl_data = pd.read_csv('<path_to_data>/NDXL_Normalised_OHLC_VWAP_VOL.csv', index_col='Date', parse_dates=True)
```

## Contributing

Contributions to enhance the analysis or improve the efficiency of the Kalman Filter implementation are welcome. Please fork the repository and submit a pull request with your changes.



























