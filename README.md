# 📈 Predicting Stock Prices

A time series machine learning project for predicting stock prices using historical market data, built with Python in a Jupyter Notebook environment.

---

## 📌 Overview

Stock price prediction is one of the most challenging and sought-after problems in quantitative finance. This project explores how machine learning and deep learning techniques can be applied to historical stock market data to model price trends and generate future predictions.

Rather than treating this as a "get-rich-quick" tool, the focus is on understanding **how models learn from sequential financial data** — the patterns, pitfalls, and limitations involved in time series forecasting.

---

## 🚀 Features

- Fetching and processing historical stock market data
- Exploratory Data Analysis (EDA) with trend and volume visualizations
- Feature engineering from time series (moving averages, returns, etc.)
- Training and evaluating regression/deep learning models
- Comparing predicted vs actual stock prices
- Evaluation using MAE, RMSE, and directional accuracy

---

## 🧪 Dataset

Historical stock data is sourced from public financial APIs or datasets, including fields such as:

| Column | Description |
|--------|-------------|
| Date | Trading date |
| Open | Opening price |
| High | Highest price of the day |
| Low | Lowest price of the day |
| Close | Closing price (target variable) |
| Volume | Number of shares traded |
| Adj Close | Adjusted closing price |

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Jupyter Notebook | Interactive development environment |
| Pandas | Data manipulation and time series handling |
| NumPy | Numerical computation |
| Scikit-learn | Preprocessing and baseline ML models |
| Keras / TensorFlow | Deep learning models (LSTM) |
| Matplotlib / Seaborn | Visualization of trends and predictions |
| yfinance / CSV | Stock data acquisition |

---

## 📁 Project Structure

```
Predicting-Stock-Prices/
│
├── predicting-stock-prices.ipynb   # Main notebook: EDA, modeling, evaluation
└── README.md
```

---

## ⚙️ Getting Started

### Prerequisites

```bash
pip install pandas numpy scikit-learn tensorflow keras matplotlib seaborn yfinance jupyter
```

### Run the Notebook

```bash
git clone https://github.com/alirezaderavi/Predicting-Stock-Prices.git
cd Predicting-Stock-Prices
jupyter notebook predicting-stock-prices.ipynb
```

---

## 📊 Workflow

1. **Data Collection** — Load historical OHLCV stock data (e.g. via yfinance or CSV)
2. **EDA** — Visualize price trends, volume, moving averages, and return distributions
3. **Feature Engineering** — Create lag features, rolling statistics, and technical indicators
4. **Preprocessing** — Normalize data using MinMaxScaler for model compatibility
5. **Modeling** — Train time series models (e.g. LSTM, Linear Regression, or similar)
6. **Evaluation** — Compare predictions vs actuals; compute MAE, RMSE
7. **Visualization** — Plot predicted vs real prices on a time axis

---

## 🔍 Key Considerations

> ⚠️ **Disclaimer:** This project is built for **educational and research purposes only**. Stock markets are highly non-deterministic and are influenced by countless external factors (news, geopolitics, sentiment) that no model can fully capture. Predictions should **never** be used as financial advice.

- **Overfitting risk** is high with time series — always evaluate on an unseen test window
- **Data leakage** is a common pitfall; ensure the train/test split respects temporal ordering
- **Stationarity** of the time series affects model performance significantly

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open a pull request or issue.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

## 👤 Author

**Alireza Deravi**  
[GitHub](https://github.com/alirezaderavi)
