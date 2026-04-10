# 📊 Stock Market Prediction Using Machine Learning

## 👤 Name: Chris Hu

---

# 📌 Table of Contents
- 📖 Overview
- 📂 Dataset Description
- ⚙️ Data Preprocessing & Feature Engineering
- ❓ Research Questions
- 🤖 Machine Learning Models
- 📊 Visualizations
- 📏 Evaluation Metrics
- 📌 Key Findings
- ⚠️ Limitations
- 🚀 Future Improvements
- 🧠 Tools Used

---

# 📖 Overview

This project explores whether machine learning models can use historical stock market data to predict future stock behavior.

We aim to determine whether past price patterns can help:

- 📈 Predict if a stock will go **up or down the next day**
- 💰 Predict the **next day’s closing price**

Dataset used:

:contentReference[oaicite:0]{index=0}

---

# 📂 Dataset Description

The dataset contains daily stock market data for multiple companies.

## 📊 Features:
- Open price  
- High price  
- Low price  
- Close price  
- Volume  
- Ticker (stock symbol)  
- Date  

---

## 📌 Target Variables Created:
- `price_up` → 1 if price increases next day, else 0  
- `next_close` → next day closing price  

---

# ⚙️ Data Preprocessing & Feature Engineering

To prepare the dataset for machine learning:

## 🔧 Steps performed:
- Sorted data by stock and date  
- Removed missing values  
- Created lag-based prediction target (`next_close`)  
- Converted problem into classification + regression tasks  
- Selected features:
  - Open  
  - High  
  - Low  
  - Close  

---

# ❓ Research Questions

## 🔹 Question 1: Classification
Can we predict whether a stock will go up or down the next day using historical price data?

- Output:
  - `1` → Price goes up  
  - `0` → Price goes down  

---

## 🔹 Question 2: Regression
Can past stock prices be used to predict the next day’s closing price?

- Output:
  - Continuous numerical value (next closing price)

---

# 🤖 Machine Learning Models

We used two supervised learning techniques:

## 📌 Classification Model
- Logistic Regression  
- Purpose: Predict stock direction (up/down)

## 📌 Regression Model
- Linear Regression  
- Purpose: Predict next closing price  

---

# 📊 Visualizations

## 📈 Visualization 1: Stock Price Trend
- Shows how stock prices change over time  
- Helps identify trends and volatility  

🧠 Includes:
- X-axis: Date  
- Y-axis: Closing Price  

---

## 📉 Visualization 2: Actual vs Predicted Prices
- Compares model predictions vs real values  
- Evaluates regression performance  

🧠 Includes:
- X-axis: Actual price  
- Y-axis: Predicted price  

---

# 📏 Evaluation Metrics

## 📌 Classification:
- Accuracy Score  
  - Measures how often the model predicts correctly  

## 📌 Regression:
- RMSE (Root Mean Squared Error)  
  - Measures average prediction error  

---

# 📌 Key Findings

- Stock movement is **partially predictable** using historical price data  
- Models capture basic patterns but struggle with volatility  
- Market behavior is highly influenced by external factors not included in the dataset  

---

# ⚠️ Limitations

- No news or sentiment data included  
- No macroeconomic indicators  
- Simple models used (no deep learning or advanced forecasting)  
- Stock market is highly unpredictable  

---

# 🚀 Future Improvements

- Add technical indicators (RSI, MACD, Moving Averages)  
- Use advanced models (Random Forest, XGBoost, LSTM)  
- Include financial news sentiment analysis  
- Improve time-series modeling techniques  

---

# 🧠 Tools Used

- Python 🐍  
- Pandas  
- NumPy  
- Matplotlib  
- Scikit-learn

AI-assisted README

---

# 📌 Summary

This project demonstrates how machine learning can be applied to financial data, while also highlighting the limitations of predicting complex real-world systems like the stock market.
