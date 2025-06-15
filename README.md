#  Financial Time-Series Anomaly Detection

##  Project Overview

This project focuses on detecting anomalies in **financial time-series data**, specifically stock price trends. The primary goal is to identify unusual behavior or outliers in stock movement that could signal major events, fraud, or trading opportunities.

We use a combination of statistical techniques and machine learning algorithms to analyze historical stock price data and flag anomalies in trends, volatility, and price fluctuations.

---

##  Objectives

- Load and preprocess historical stock market data
- Calculate key financial indicators (moving averages, volatility, returns)
- Apply anomaly detection algorithms (Isolation Forest, DBSCAN)
- Forecast trends using LSTM or Prophet
- Visualize anomalies and prediction uncertainty

---

##  Dataset

- **Source**: Yahoo Finance API
- **Sample Ticker**: AAPL, MSFT, TSLA, etc.
- **Time Period**: Adjustable (e.g., last 5 years)
- **Features Used**:
  - `Open`, `High`, `Low`, `Close`, `Volume`
  - Technical indicators (Moving Average, RSI, Volatility, etc.)

> You can change the ticker and time range to analyze different stocks.

---

##  Technologies Used

- **Python**
  - `pandas`, `numpy` – data manipulation
  - `matplotlib`, `seaborn`, `plotly` – visualization
  - `scikit-learn` – Isolation Forest, DBSCAN
  - `tensorflow` / `keras` – LSTM (forecasting)
  - `prophet` – Facebook Prophet time-series model
- **yfinance** – fetch real-time and historical stock data

---

##  Project Workflow

1. **Data Collection**
   - Fetch historical stock data using `yfinance`

2. **Preprocessing**
   - Handle missing values, compute log returns
   - Calculate rolling averages and volatility

3. **Anomaly Detection**
   - Apply `Isolation Forest` and/or `DBSCAN` on engineered features
   - Label points as anomalous or normal

4. **Forecasting**
   - Use LSTM or Prophet to model and forecast future stock trends
   - Evaluate using RMSE, MAE

5. **Visualization**
   - Plot stock prices with anomalies highlighted
   - Forecast with uncertainty intervals

---

##  Results & Insights

- Successfully detected price spikes/drops using **Isolation Forest**
- **DBSCAN** detected density-based outliers in low-volume periods
- **Prophet** forecasted trends with seasonality and trend changepoints
- **LSTM** showed potential for multi-step forecasting but required tuning

> Anomalies can help in building alert systems for financial risk or trading signals.

---

---

##  How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/financial-anomaly-detection.git
   cd financial-anomaly-detection
