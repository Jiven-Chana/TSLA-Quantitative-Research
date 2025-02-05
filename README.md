# 🚀 Kalman Filter & Monte Carlo Simulation for TSLA Stock Forecasting

## 📌 Overview

This repository contains Python implementations of **Kalman Filtering** and **Monte Carlo Simulation** for forecasting **Tesla (TSLA) stock prices**. By integrating **real-time financial data**, these models estimate stock price dynamics, analyze market sensitivity, and generate probabilistic future price distributions.

### 🔹 Key Features
- **Kalman Filter for Real-Time State Estimation**
  - Dynamically estimates **Tesla’s stock price movements** relative to a market composite index.
  - Computes **rolling alpha & beta** to assess Tesla’s sensitivity to broader market fluctuations.
  - Uses **VWAP, volatility, and closing prices** as key input variables.

- **Monte Carlo Simulation with Geometric Brownian Motion (GBM)**
  - Forecasts future price movements using **stochastic modeling**.
  - Runs **10,000+ simulations** to generate **probabilistic price distributions**.
  - Evaluates market volatility impact through **sensitivity heatmaps**.

- **Comprehensive Financial Data Integration**
  - Utilizes **daily Tesla stock data** and a composite index (*NDXL*).
  - Incorporates **Nasdaq 100 (NDX), Consumer Discretionary (XLY), Autonomous EVs (DRIV), and Lithium Tech (LIT)** to track sector-specific influences.

---

---

## 🛠 Installation & Dependencies

Ensure you have the following dependencies installed:

```bash
pip install numpy pandas matplotlib scipy yfinance scikit-learn
```

Additionally, install Jupyter Notebook for interactive analysis:

```bash
pip install notebook
```

---

---

## 🚀 Usage Guide

### 🔹 1. Running the Kalman Filter
To estimate **Tesla’s market sensitivity**:

```bash

```

This will output:
- **Rolling Alpha & Beta estimates** for Tesla.
- **Time-series plots** comparing Tesla’s stock behavior against its market composite.

### 🔹 2. Running Monte Carlo Simulation
To simulate **future Tesla stock price paths**:

```bash

```

This will generate:
- **Multiple simulated price paths** for different time horizons (3 months, 6 months, 1 year, 5 years).
- **Probability distributions & confidence intervals** for price forecasts.
- **Sensitivity heatmaps** analyzing the impact of volatility changes.

---

## 📊 Key Outputs

### 📈 Simulated Price Paths
- **Forecasts Tesla’s stock trajectory** based on historical drift & volatility.
- Provides **confidence bands** for price expectations.

### 🎯 Rolling Beta & Alpha Analysis
- **Beta:** Measures Tesla’s **market sensitivity**—a high beta suggests Tesla moves in sync with broader markets.
- **Alpha:** Measures **Tesla’s independent performance**—a negative trend suggests underperformance relative to market risk.

### 🔥 Sensitivity Heatmaps
- Shows how **changes in volatility (σ) & drift (µ)** impact Tesla’s price projections.
- Helps investors fine-tune **risk management & trading strategies**.

---

## 📌 Model Assumptions & Limitations

### 🔹 Kalman Filter Considerations
✔ Assumes **Tesla’s market behavior follows a dynamic regression model**.  
✔ Uses **daily VWAP, volatility, and returns** to update state estimates.  
⚠ Performance depends on **data accuracy & feature engineering**.

### 🔹 Monte Carlo Simulation Assumptions
✔ Uses **Geometric Brownian Motion (GBM)**, assuming **log-normal price distribution**.  
✔ Generates **10,000+ stochastic price paths** to model **uncertainty & volatility**.  
⚠ Does not account for **market shocks, economic policy changes, or black swan events**.

---

## 📈 Investment Insights

This project provides **quantitative insights** for investors and analysts by:
- **Assessing Tesla’s risk & volatility profile** through **rolling beta analysis**.
- **Forecasting potential price ranges** using **Monte Carlo simulation**.
- **Enhancing trading strategies** with **dynamic market sensitivity tracking**.

---

## 🤝 Contributing

We welcome contributions to improve:
- **Model accuracy & feature selection** for Kalman Filter.
- **Alternative stochastic models** beyond GBM for Monte Carlo simulations.
- **New visualizations & statistical metrics** for enhanced analysis.

To contribute, **fork the repository** and submit a **pull request**.

---

## 📜 License

This project is licensed under the **MIT License** – feel free to use and modify.

---

## 📩 Contact & Support

For any inquiries, reach out via **GitHub Issues** or email 📧 *jiven.chana@icloud.com*.


