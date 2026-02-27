# Trader Performance vs Market Sentiment Analysis

## Project Overview
This project analyzes the relationship between Bitcoin market sentiment (Fear vs Greed) and trader behavior on Hyperliquid.  
The goal is to identify patterns in trading performance and behavioral changes across sentiment regimes and derive actionable insights for sentiment-aware trading strategies.

---

## Objective
- Evaluate how trader profitability changes with market sentiment  
- Analyze behavioral shifts such as leverage, trade frequency, and position sizing  
- Identify trader segments based on risk exposure and activity  
- Propose actionable strategy ideas based on observed patterns  

---

## Datasets

### 1️⃣ Bitcoin Fear & Greed Index
- Columns: Date, Classification  
- Used to label the market sentiment regime  

### 2️⃣ Historical Trader Data
Includes trading activity on Hyperliquid with fields such as:
- Account  
- Execution price  
- Side  
- Size USD  
- Closed PnL  
- Leverage  
- Timestamp  

---

## 🧹 Data Preparation

- Checked dataset dimensions, missing values, and duplicates  
- Converted trade timestamps to daily level  
- Aggregated metrics per account per day  
- Filtered sentiment data to match the trading date range  
- Merged sentiment classification with trader metrics  

This ensured consistent temporal alignment and reliable analysis.

---

## ⚙️ Methodology

1. Loaded both datasets and performed data quality checks  
2. Converted timestamps to daily granularity  
3. Aggregated trader metrics per account per day  
4. Created key features:
   - Daily PnL  
   - Win rate  
   - Average trade size  
   - Trade frequency  
   - Average leverage  
5. Merged trader metrics with sentiment classification  
6. Conducted comparative analysis across sentiment regimes  
7. Segmented traders based on activity and leverage  

---

## 📊 Key Metrics

- Daily PnL per account  
- Win rate  
- Trades per day  
- Average trade size  
- Average leverage  
- Sentiment classification  

---

## 🔍 Key Insights

1. **Risk-taking increases during Greed periods**  
   Traders exhibit higher leverage and trading activity, indicating stronger confidence and momentum-driven behavior.

2. **Market Fear introduces higher variability in performance**  
   Profitability dispersion increases, suggesting unstable and volatile trading conditions.

3. **High-frequency traders adapt better to sentiment changes**  
   Active traders maintain relatively stable performance compared to infrequent traders.

4. **Leverage is strongly correlated with PnL volatility**  
   Higher leverage leads to larger gains but also significantly larger losses, highlighting risk concentration.

---

## 👥 Trader Segmentation

To better understand behavioral differences, traders were segmented based on:

- Activity level (high vs low trade frequency)  
- Risk exposure (high vs low leverage)  
- Performance stability (consistent vs volatile PnL)  

Segment analysis shows that high-frequency traders adapt better across sentiment regimes, while high-leverage traders experience larger performance swings.

---

## 🚀 Strategy Recommendations

1. **Dynamic Leverage Adjustment**  
   Reduce leverage exposure during Fear regimes to manage downside risk and volatility.

2. **Momentum Participation Strategy**  
   Increase trading activity during Greed phases for traders with strong historical win rates.

3. **Risk-Based Segmentation**  
   Allow higher exposure for consistent performers while capping leverage for volatile traders.

4. **Sentiment as Risk Filter**  
   Use sentiment signals to adjust position sizing rather than as a standalone trading signal.

---

## ▶️ How to Run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook notebook.ipynb
```

## 📁 Project Structure

project-folder/
│
├── notebook.ipynb
├── historical_data.csv
├── fear_greed_index.csv
├── outputs/
│   ├── charts
├── report.pdf
└── README.md

## 🧾 Conclusion

The analysis demonstrates a clear relationship between market sentiment and trader behavior.
Incorporating sentiment signals into risk management frameworks can help improve decision-making, optimize exposure, and enhance trading performance.
