# Monte Carlo Simulation for TSLA Stock Price Forecasting

## Overview

This repository contains a Python-based Monte Carlo simulation model for forecasting Tesla Inc. (TSLA) stock price movements. The model applies **Geometric Brownian Motion (GBM)** to simulate multiple future price trajectories, providing a probabilistic forecast of potential stock price distributions. This approach helps investors assess uncertainty and evaluate risk in future price movements.

## Features

The script performs the following key functions:

### 📊 **Data Handling**
- Loads **historical TSLA stock price data** and related market indices.
- Cleans, processes, and prepares data for modeling.

### 📈 **Geometric Brownian Motion (GBM)**
- Estimates **drift** (expected return) and **volatility** from historical price movements.
- Simulates multiple possible future price paths for TSLA stock.

### 🎲 **Monte Carlo Simulation**
- Runs a large number of simulations to generate probabilistic price forecasts.
- Uses **randomized sampling** to model uncertainty in future stock movements.

### 📉 **Visualization**
- Plots **simulated price trajectories** to showcase potential market scenarios.
- Generates **histograms** of projected stock price distributions.

### 📊 **Statistical Analysis**
- Computes **expected future price ranges** and probability intervals.
- Evaluates **confidence intervals** and risk metrics.

---

## 📁 Project Structure

```plaintext
├── data/        # Historical stock price data (CSV files)
├── notebooks/   # Jupyter notebooks for in-depth analysis & visualization
├── src/         # Source code for Monte Carlo simulations
├── results/     # Outputs from simulations (e.g., plots, statistical summaries)
├── README.md    # Project documentation
└── monte_carlo_simulation.py  # Main script
```

---

## 🚀 Usage

### **1. Install Dependencies**
Ensure you have the required libraries installed before running the script:

```bash
pip install numpy pandas matplotlib scipy yfinance
```

## Run the Simulation

Navigate to the project directory and execute the script:

```bash
python monte_carlo_simulation.py
```

## Modify Parameters

You can customize key simulation parameters in the script:

```python
num_simulations = 10000  # Number of Monte Carlo iterations
time_horizon = 252       # Forecasting horizon in trading days
```

## 📊 Visualizations

The script generates several insightful visualizations:
	•	Simulated Price Paths: Multiple potential future price trajectories.
	•	Probability Distribution: Histogram showing the likelihood of different price levels.
	•	Statistical Insights: Confidence intervals and expected price ranges.








