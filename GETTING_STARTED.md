# Getting Started Guide

## Welcome to Hyperliquid Sentiment & Behavioral Analysis! 🚀

This guide will help you get up and running with the project in minutes. Whether you're a developer, analyst, or trader, follow these steps to explore Bitcoin market sentiment's impact on trading performance.

## 📋 Prerequisites

Before you begin, ensure you have:

- **Python 3.8 or higher** installed on your system
- **Git** for version control
- **A modern web browser** (Chrome, Firefox, Safari, Edge)
- **At least 2GB free disk space** for data and dependencies

## 🔧 Quick Setup (5 minutes)

### 1. Clone the Repository

```bash
git clone https://github.com/ykjaat6104/Hyperliquid-Sentiment-and-Behavioral-Analysis.git
cd Hyperliquid-Sentiment-and-Behavioral-Analysis
```

### 2. Set Up Virtual Environment

```bash
# Create virtual environment
python -m venv .venv

# Activate it
# On Windows:
.venv\Scripts\activate
# On macOS/Linux:
source .venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Prepare Data

Place your data files in the `input/` directory:

- `fear_greed_index.csv`: Fear/Greed Index data
- `historical_data.csv`: Hyperliquid trading data

If you don't have the data files, the app will show an error message.

### 5. Launch the Dashboard

```bash
streamlit run app.py
```

Open http://localhost:8501 in your browser and start exploring!

## 🎯 First Steps

### Explore the Dashboard

1. **🏠 Overview Page**: Get a high-level view of key metrics and sentiment distribution
2. **📊 Performance Page**: Dive deep into performance analytics by sentiment
3. **🎯 Strategies Page**: Discover actionable trading strategies

### Run the Analysis Notebook

For detailed analysis and customization:

```bash
jupyter notebook Hyperliquid_analysis.ipynb
```

## 📊 Understanding the Data

### Fear/Greed Index
- **Source**: alternative.me API
- **Format**: Daily sentiment scores (0-100) with classifications
- **Categories**: Extreme Fear, Fear, Neutral, Greed, Extreme Greed

### Trading Data
- **Source**: Hyperliquid exchange
- **Anonymized**: Trader accounts are hashed for privacy
- **Metrics**: PnL, trade size, timestamps, position types

## 🛠️ Troubleshooting

### Common Issues

**"Error loading data"**
- Ensure CSV files are in `input/` directory
- Check file formats match expectations
- Verify data dates align

**"Streamlit not found"**
- Ensure virtual environment is activated
- Run `pip install -r requirements.txt` again

**"Port 8501 already in use"**
- Close other Streamlit apps or use a different port: `streamlit run app.py --server.port 8502`

### Getting Help

- Check the README.md for detailed documentation
- Review the Jupyter notebook for analysis methodology
- Open an issue on GitHub for bugs or feature requests

## 🚀 Next Steps

Once you're set up:

1. **Explore the Dashboard**: Navigate through different pages to understand the insights
2. **Customize Analysis**: Modify the notebook for your own data or parameters
3. **Build Strategies**: Use the findings to develop your own trading rules
4. **Contribute**: Fork the repo and submit pull requests for improvements

Happy analyzing! 📈💹
