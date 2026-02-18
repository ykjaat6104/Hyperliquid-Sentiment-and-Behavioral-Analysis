# Hyperliquid Sentiment & Behavioral Analysis 📊💹

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![Streamlit](https://img.shields.io/badge/Streamlit-1.28+-red.svg)](https://streamlit.io)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> **Professional Quantitative Analysis**: How Bitcoin market sentiment (Fear/Greed Index) impacts trader behavior and performance on Hyperliquid. Built with 200K+ real trades from 32 traders over 2+ years.

## 🎯 Overview

This project performs quantitative analysis on the relationship between Bitcoin market sentiment and trading performance on Hyperliquid. It addresses three critical questions:

1. **Performance Impact**: Does PnL differ between Fear vs Greed market conditions?
2. **Behavioral Adaptation**: Do traders unconsciously change their behavior based on sentiment?
3. **Optimal Segments**: Which trader types (frequency, consistency) perform best under different conditions?

## 🏗️ System Architecture

```
historical_data.csv  ──┐
                        ├──► Load ──► Clean ──► df_merged
fear_greed_index.csv ──┘                            │
                                                    ▼
                                          Metrics Aggregation
                                          (daily_metrics)
                                                    │
                          ┌─────────────────────────┼──────────────────────┐
                          ▼                          ▼                      ▼
                    Analysis (Part B)        Segmentation           Visualization
                    sentiment_perf           user_segments          (Part C charts)
                                                    │
                                          ┌─────────┤
                                          ▼         ▼
                                     Clustering  Prediction
                                     (Bonus)     (Bonus)
                                          │
                                          ▼
                                    Strategy Rules
                                    (Part D)
```

## 📁 Project Structure

```
Hyperliquid Analysis/
├── .gitignore
├── LICENSE
├── README.md
├── GETTING_STARTED.md
├── app.py
├── Hyperliquid_analysis.ipynb
├── pyproject.toml
├── requirements.txt
├── .venv/
│   └── (virtual environment files)
└── input/
    ├── fear_greed_index.csv
    └── historical_data.csv
```

## ✨ Features

- **Interactive Dashboard**: Streamlit web app for exploring real-time insights and visualizations
- **Sentiment Analysis**: Integration of Fear/Greed Index with historical trading data
- **Performance Metrics**: Daily PnL, win rates, trade counts segmented by sentiment levels
- **Behavioral Clustering**: K-means clustering to identify trader archetypes and patterns
- **Strategy Recommendations**: Evidence-based trading strategies tailored to sentiment conditions
- **Statistical Validation**: T-tests, correlations, and significance testing for robust analysis

## � Project Outputs


- **Sentiment Performance**: 
  <img width="4153" height="2353" alt="sentiment_performance" src="https://github.com/user-attachments/assets/01f97b19-8306-4dae-bcea-e1ed6e1a24e8" />

- **PCA Projection & Traders Archetype**:
  <img width="2100" height="900" alt="trader_archetypes" src="https://github.com/user-attachments/assets/bacefcb4-71b8-40e6-9ef3-be52d136b2c7" />

- **Elbow Method Results**:
  <img width="1200" height="750" alt="elbow_method" src="https://github.com/user-attachments/assets/cddf1b6f-ee76-4427-bba1-90a27a4fe612" />
 
## �🚀 Quick Start

### Prerequisites

- Python 3.8+
- Git

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/ykjaat6104/Hyperliquid-Sentiment-and-Behavioral-Analysis.git
   cd Hyperliquid-Sentiment-and-Behavioral-Analysis
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

- **Fear/Greed Index**: Alternative.me API providing daily sentiment scores (0-100) with classifications
- **Trading Data**: Hyperliquid historical trade data (anonymized for privacy)

Place CSV files in the `input/` directory:
- `fear_greed_index.csv`: Columns - Date, Value, Classification
- `historical_data.csv`: Columns - Timestamp, Account, Closed PnL, Size USD, etc.

## 🔍 Methodology

1. **Data Integration**: Merge sentiment data with trader performance metrics by date
2. **Sentiment Segmentation**: Classify trading days into Fear, Neutral, and Greed periods
3. **Performance Analysis**: Compare PnL, win rates, and trade volumes across sentiment groups
4. **Behavioral Clustering**: Apply K-means to segment traders by frequency and consistency
5. **Strategy Development**: Formulate evidence-based rules for sentiment-aware trading

## 📈 Key Findings

- Greed days show 56.5% underperformance vs Fear days
- Traders reduce trade frequency by 72.1% during Greed periods
- Infrequent traders outperform frequent ones on Fear days
- Quality filtering improves win rates by 3.1 percentage points

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch 
3. Commit your changes 
4. Push to the branch
5. Open a Pull Request

## 📄 License

MIT License - see LICENSE file for details

## 📧 Contact

For questions or collaborations, reach out!

---

*Built with ❤️ for quantitative trading insights*
