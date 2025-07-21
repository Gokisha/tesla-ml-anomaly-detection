# 🚨 Tesla Intraday Anomaly Detection using Isolation Forest

This project uses machine learning to detect anomalous price movements in **Tesla's intraday stock data**. It leverages the **Isolation Forest** algorithm to flag outliers in price and volume — helping identify unusual market activity, potential manipulation, or high-volatility periods.

---

## 📌 Project Overview

- **Objective**: Detect anomalies in Tesla’s 1-hour interval trading data using an unsupervised learning model.
- **Data Source**: [Yahoo Finance](https://finance.yahoo.com/quote/TSLA) via `yfinance` Python package.
- **Interval**: Intraday (1-hour) data over the past 365 days.
- **Tech Stack**: Python, Pandas, Scikit-learn, Matplotlib, yfinance.

---

## 💡 Why Anomaly Detection in FinTech?

Anomaly detection is widely used in financial systems for:
- Spotting **suspicious market activity**
- Detecting **flash crashes or manipulation**
- Supporting **quantitative trading strategies**
- Enabling **risk monitoring and fraud detection**

This project simulates such a use case by applying anomaly detection on real intraday price data.

---

## 🔍 Methodology

1. **Download Data**:
   - Tesla (TSLA) intraday data with 1-hour resolution using `yfinance`.
2. **Preprocessing**:
   - Remove empty rows
   - Standardize timestamp and numeric columns
3. **Anomaly Detection**:
   - Use **Isolation Forest** on selected features (`Open`, `High`, `Low`, `Close`, `Volume`)
   - Classify each row as normal or anomalous
4. **Visualization**:
   - Highlight anomalies on a time-series price plot

