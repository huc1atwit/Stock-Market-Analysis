# 📊 Stock Market Prediction Using Machine Learning

## 👤 Name: Chris Hu

---

## 📌 Project Overview

This project explores whether machine learning models can use historical stock market data to:

1. Predict whether a stock will go **up or down the next day**
2. Predict the **next day’s closing price**

We use real-world stock data from the Hugging Face dataset:

["dataset","Stocks Daily Price Dataset","Hugging Face paperswithbacktest dataset"]

This dataset includes daily stock values such as:

* Open price
* High price
* Low price
* Close price
* Trading volume

---

## ❓ Research Questions

### 1. Classification Question

**Can we predict whether a stock will go up or down the next day using past price data?**

* Output:

  * 1 = price goes up
  * 0 = price goes down

---

### 2. Regression Question

**Can past stock prices be used to predict the next day’s closing price of a stock?**

* Output:

  * Continuous value (next day closing price)

---

## 📂 Dataset Description

The dataset contains daily stock market data for multiple companies.

### Features used in this project:

* Open
* High
* Low
* Close

### Target variables created:

* `price_up` → classification target
* `next_close` → regression target

---

## ⚙️ Methodology

### 1. Data Preprocessing

* Sorted data by ticker and date
* Created lag-based target variables:

  * Next day closing price
  * Price direction (up/down)
* Removed missing values

---

### 2. Machine Learning Models

#### 📌 Classification Model

* Logistic Regression
* Goal: Predict stock movement direction

#### 📌 Regression Model

* Linear Regression
* Goal: Predict next day closing price

---

## 📊 Visualizations

### 📈 1. Stock Price Trend Over Time

* Shows how a stock’s closing price changes over time
* Helps visualize volatility and trends

### 📉 2. Actual vs Predicted Prices

* Compares predicted closing prices vs real values
* Shows model performance visually

---

## 📏 Evaluation Metrics

### Classification

* Accuracy Score

### Regression

* Root Mean Squared Error (RMSE)

---

## 📌 Key Findings

* Stock price direction is **partially predictable** using historical data
* Linear models can capture basic trends but struggle with volatility
* Stock markets are influenced by external factors not included in the dataset

---

## ⚠️ Limitations

* Only uses price-based features (no news or sentiment data)
* Does not account for macroeconomic factors
* Models assume past trends continue into the future

---

## 🚀 Future Improvements

* Add technical indicators (RSI, Moving Averages)
* Use advanced models (Random Forest, LSTM, XGBoost)
* Include sentiment analysis from financial news

---

## 🧠 Tools Used

* Python
* Pandas
* NumPy
* Scikit-learn
* Matplotlib
