# 📈 Algotrading With Sentiment Analysis

A real-time stock price monitoring and prediction pipeline built with Python, designed for high-frequency trading and dynamic financial analysis using machine learning techniques and sentiment-driven insights.

![stock-header](https://img.shields.io/badge/Python-3.9-blue.svg) ![license](https://img.shields.io/badge/license-MIT-green)

---

## 🚀 Features

* 📊 **Real-time Stock Data Collection** using the Yahoo Finance API (`yfinance`)
* 🧹 **Data Preprocessing** with datetime formatting, missing-value handling, normalization
* 🧠 Ready for **ML Model Integration** (LSTM, XGBoost, Linear Regression)
* 🧱 **Modular Design** for ease of testing, scaling, and extension
* 💾 **Data Saving** as clean CSVs for downstream analytics
* 📉 Exploratory Analysis: Trend visualization, volatility, technical indicators
* 📦 Two working notebooks:

  * `5stocks.ipynb` – fetches and processes multiple stock data
  * `marketstocks.ipynb` – customizable real-time stock data pipeline

---

## 📂 Project Structure

```
.
├── 5stocks.ipynb
├── marketstocks.ipynb
├── GenAI_Report_Group_9.pdf  # Detailed project report
├── requirements.txt
└── README.md
```

---

## 🏗️ Pipeline Components

| Function                | Description                                                     |
| ----------------------- | --------------------------------------------------------------- |
| `get_live_stock_data()` | Fetches OHLCV data from Yahoo Finance                           |
| `preprocess_data()`     | Cleans data: datetime conversion, missing value treatment, etc. |
| `save_data()`           | Saves cleaned data to CSV                                       |
| `run_pipeline()`        | Orchestrates full flow: fetch → preprocess → save               |

---

## 📈 Exploratory Analysis Examples

* 📍 Trend & volatility plots (OHLC, rolling std deviation)
* 🔁 Technical indicators like RSI, MACD, Moving Averages
* 📌 Correlation heatmaps
* 📦 Histogram and distribution plots for returns

---

## 📚 Future Enhancements

* 🤖 Integrate ML models like LSTM or XGBoost for forecasting
* 📊 Build interactive dashboards with **Streamlit** or **Dash**
* 🔔 Real-time alerts for trade signals or major price shifts
* 💬 Integrate **news sentiment analysis** for smarter predictions

---

## 🔧 Installation & Setup

```bash
git clone https://github.com/yourusername/Algotrading-Sentiment.git
cd Algotrading-Sentiment
pip install -r requirements.txt
```

---

## 📋 Usage

In `marketstocks.ipynb`, change:

```python
ticker = 'TCS.NS'
interval = '1d'
```

Run the pipeline:

```python
run_pipeline(ticker, interval, save_path='TCS_cleaned.csv')
```

To analyze multiple stocks, use `5stocks.ipynb`.

---

## 📄 Report

For complete methodology, literature review, and diagrams, see [GenAI\_Report\_Group\_9.pdf](./GenAI_Report_Group_9.pdf).

---

## 🧠 Authors

* Anshul Yadav
* Shruti Bajpayee
* Saransh Bhargava
* Ritika Yadav
  *Mentored by Dr. Manisha Saini, BML Munjal University*

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).
