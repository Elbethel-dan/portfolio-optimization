# 📈 Time Series Forecasting for Portfolio Management
---
## 🎯 Project Objective

This project applies time series analysis and forecasting techniques to historical financial data in support of portfolio management at Guide Me in Finance (GMF) Investments. Using real-world market data sourced from YFinance, the analysis explores asset price behavior, returns, volatility, and risk to generate actionable insights for investment decision-making. In alignment with the Efficient Market Hypothesis, forecasting models in this project are treated as analytical tools to identify trends, momentum, and risk patterns rather than as mechanisms for exact price prediction. The results are intended to complement broader portfolio strategies by helping analysts evaluate market conditions, optimize asset allocation, and manage investment risk more effectively.

---
## 📊 Task 1: Financial Data Analysis & Market Insight Discovery

In this task, historical market data for BND, SPY, and TSLA are collected using YFinance and prepared for analysis. The focus is on understanding price behavior, return dynamics, and risk characteristics across different asset classes. Exploratory Data Analysis (EDA) is conducted to visualize trends, assess volatility, identify outliers, and examine daily returns. Statistical summaries and risk metrics such as volatility, Value at Risk (VaR), and Sharpe Ratio are used to compare asset performance and risk profiles. This analysis provides a strong analytical foundation for informed portfolio decisions and model development.

---
## 📈 Task 2: Task 2: Time Series Forecasting & Modeling

This task focuses on forecasting Tesla’s stock behavior using both classical and deep learning models. ARIMA/SARIMA models are applied to prices and returns after assessing stationarity and temporal structure, while an LSTM neural network is implemented to capture nonlinear patterns and long-term dependencies in the data. Models are trained using chronological splits and evaluated with MAE, RMSE, and MAPE. Performance comparisons highlight trade-offs between interpretability and predictive flexibility, reinforcing the role of forecasting models as decision-support tools rather than exact price predictors.

---
## 🔮 Task 3: Forecast Future Market Trends

Building on the best-performing model from Task 2, this task generates 12-month forward-looking forecasts for Tesla's stock price with quantified uncertainty bounds. The ARIMA model trained on returns data produces future price projections with 95% confidence intervals, revealing a flat-to-slightly-negative trend with high volatility. Visualizations distinguish between historical data, test predictions, and future forecasts, while trend analysis examines how uncertainty widens over longer horizons following a √t pattern. The analysis translates forecasts into market opportunities and risks, providing actionable insights for portfolio positioning and risk management strategies.

---
## ⚖️ Task 4: Portfolio Optimization Based on Forecast
This task applies Modern Portfolio Theory (MPT) to construct an optimal asset allocation using the Tesla forecast as a specific "view" while incorporating historical data for SPY and BND. The expected returns vector combines forecasted Tesla returns with historical averages for SPY and BND, while the covariance matrix captures historical relationships. The efficient frontier is generated through simulation, identifying the Maximum Sharpe Ratio and Minimum Volatility portfolios. Visualization includes the efficient frontier plot, covariance matrix heatmaps, and portfolio weight comparisons, culminating in a recommended portfolio allocation with justification based on risk-adjusted return optimization.

---

## 📉 Task 5: Strategy Backtesting
The final task validates the optimized portfolio strategy through historical simulation on the 2025-2026 test period. The strategy portfolio (using weights from Task 4) is compared against a 60/40 SPY/BND benchmark portfolio, testing both buy-and-hold and monthly rebalancing approaches. Performance metrics including total return, annualized return, Sharpe ratio, and maximum drawdown are calculated for comparison. Comprehensive visualizations show cumulative returns, drawdowns, and rolling performance metrics, while statistical tests assess significance of outperformance. The backtest concludes with a viability assessment of the model-driven approach and discussion of implementation limitations.

---


## ⚙️ Reproduce this environment

To set up and reproduce this project locally, follow the steps below:

## 1. Clone the repository
```bash
   git clone https://github.com/Elbethel-dan/solar-challenge-week0.git
```
## 2. Create and activate a virtual environment (recommended)

   **For macOS / Linux**
   ```bash
     python3 -m venv week0
     source week0/bin/activate
   ```

   **For Windows**
   ```bash
     python -m venv week0
     week0\Scripts\activate
   ```
## 3. Install dependencies
  ```bash
     pip install -r requirements.txt
 ```

--- 

## 📈 Key Insights

- Tesla Forecast: Flat expected return with high volatility (3.6% daily)

- Portfolio Optimization: Balanced allocation reduces volatility by ~70% vs TSLA alone

- Backtest Results: Model-driven strategy shows moderate viability vs 60/40 benchmark

- Practical Application: Forecasting serves as decision-support, not exact prediction

--- 

## 🛠️ Technologies Used

- Data Analysis: Pandas, NumPy, SciPy

- Visualization: Matplotlib, Seaborn, Plotly

- Time Series Forecasting: Statsmodels, pmdarima

- Portfolio Optimization: CVXPY, PyPortfolioOpt

- Deep Learning: TensorFlow/Keras (LSTM)