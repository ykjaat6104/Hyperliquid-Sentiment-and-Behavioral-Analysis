# Hyperliquid Sentiment & Behavioral Analysis 📊💹

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)](https://streamlit.io)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Professional Quantitative Analysis**: How Bitcoin market sentiment (Fear/Greed Index) impacts trader behavior and performance on Hyperliquid. Built with 200K+ real trades from 32 traders over 2+ years.

## 🎯 Overview

This project performs comprehensive quantitative analysis on the relationship between Bitcoin market sentiment and trading performance. We answer three critical questions:

1. **Performance Impact**: Does PnL differ between Fear vs Greed market conditions?
2. **Behavioral Adaptation**: Do traders unconsciously change their behavior based on sentiment?
3. **Optimal Segments**: Which trader types (frequency, consistency) perform best under different conditions?

## ✨ Features

- **Interactive Dashboard**: Streamlit-based web app for real-time insights
- **Sentiment Analysis**: Fear/Greed Index integration with trading data
- **Performance Metrics**: Daily PnL, win rates, trade counts by sentiment
- **Behavioral Clustering**: K-means clustering of trader archetypes
- **Strategy Recommendations**: Actionable trading strategies based on sentiment
- **Statistical Validation**: T-tests and correlation analysis

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/hyperliquid-sentiment-analysis.git
cd hyperliquid-sentiment-analysis
```

2. Create virtual environment:
```bash
python -m venv .venv
source .venv/bin/activate  # On Windows: .venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

### Usage

#### Run the Dashboard
```bash
streamlit run app.py
```
Open http://localhost:8501 in your browser.

#### Run the Analysis Notebook
```bash
jupyter notebook Hyperliquid_analysis.ipynb
```

## 📊 Data Sources

- **Fear/Greed Index**: Alternative.me API (daily sentiment scores)
- **Trading Data**: Hyperliquid historical trade data (anonymized)

Place CSV files in the `input/` directory:
- `fear_greed_index.csv`: Date, Value, Classification
- `historical_data.csv`: Timestamp, Account, Closed PnL, Size USD, etc.

## 🔍 Analysis Methodology

1. **Data Integration**: Merge sentiment with trader performance
2. **Sentiment Segmentation**: Fear/Neutral/Greed periods
3. **Performance Analysis**: Statistical comparison of metrics
4. **Behavioral Clustering**: Trader archetypes via K-means
5. **Strategy Development**: Evidence-based trading rules

## 📈 Key Findings

- Greed days show 56.5% underperformance vs Fear days
- Traders reduce frequency by 72.1% during Greed
- Infrequent traders outperform frequent ones on Fear days
- Quality filtering improves win rates by 3.1pp

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## 📄 License

MIT License - see LICENSE file for details

## 📧 Contact

For questions or collaborations, reach out!

---

*Built with ❤️ for quantitative trading insights*
