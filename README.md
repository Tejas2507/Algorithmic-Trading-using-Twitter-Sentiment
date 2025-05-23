# 📈 Algorithmic Trading using Twitter Sentiment and Machine Learning

This project implements a basic **algorithmic trading strategy** using **Twitter sentiment analysis** combined with **machine learning** techniques. It aims to analyze public sentiment about a particular stock, classify it, and use that as a feature to predict stock movement.

---

## 📚 What This Project Does

- Scrapes tweets related to a specific stock ticker.
- Cleans and preprocesses the tweet text.
- Uses a pre-trained sentiment analysis model to label tweets as Positive, Negative, or Neutral.
- Uses machine learning (Logistic Regression) to predict stock price movement based on sentiment and market data.

---

## 🛠 Technologies Used

- `Tweepy`: For scraping Twitter data.
- `TextBlob`: For sentiment analysis.
- `scikit-learn`: For machine learning (Logistic Regression).
- `yfinance`: For fetching historical stock data.
- `pandas`, `numpy`, `matplotlib`: For data manipulation and visualization.

---

## 🧠 How It Works (Pipeline Overview)

1. **Data Collection**: Fetch tweets for a particular stock (e.g., TSLA).
2. **Sentiment Analysis**: Label each tweet using `TextBlob`.
3. **Merge with Stock Data**: Align sentiment data with daily stock movement.
4. **Feature Engineering**: Create features like rolling sentiment score, previous day’s sentiment, etc.
5. **Train ML Model**: Use features to train a Logistic Regression classifier to predict stock movement (Up/Down).
6. **Evaluate Performance**: Accuracy, confusion matrix, etc.

---

## 🚀 Getting Started

Install dependencies:

```bash
pip install tweepy textblob scikit-learn yfinance pandas matplotlib
