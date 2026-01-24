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

