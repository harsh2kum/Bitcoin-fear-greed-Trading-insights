# Bitcoin Fear-Greed vs Trader Behavior Analysis

This project analyzes the relationship between **Bitcoin market sentiment (Fear & Greed Index)** and **trader behavior** using historical trade data from **Hyperliquid**.

---

## 📌 Objective
To understand how trading behavior changes across market sentiment conditions such as:

- Extreme Fear  
- Fear  
- Neutral  
- Greed  
- Extreme Greed  

Key trader behavior metrics analyzed:
- Trading volume (USD)
- Number of trades
- Profitability (PnL)
- Win rate
- Average trade size
- Fees

---

## 📂 Dataset Details

### 1) Bitcoin Market Sentiment Dataset (Fear & Greed Index)
Columns:
- `timestamp`
- `value`
- `classification`
- `date`

### 2) Historical Trader Data (Hyperliquid)
Columns:
- `Account`
- `Coin`
- `Execution Price`
- `Size Tokens`
- `Size USD`
- `Side`
- `Timestamp IST`
- `Start Position`
- `Direction`
- `Closed PnL`
- `Transaction Hash`
- `Order ID`
- `Crossed`
- `Fee`
- `Trade ID`
- `Timestamp`

---

## 📁 Project Structure
ds_harsh_kumar/
├── notebook_1.ipynb
├── csv_files/
│ ├── historical_data.csv
│ ├── fear_greed_index.csv
│ └── merged_daily_sentiment_trading.csv (generated)
├── outputs/
│ ├── sentiment_vs_volume.png
│ ├── sentiment_vs_pnl.png
│ ├── winrate_by_sentiment.png
│ └── trade_size_by_sentiment.png
├── ds_report.pdf
└── README.md


---

## ⚙️ Setup & Requirements
Run this project using **Google Colab** or local Python.

### Libraries Used
- Python 
- pandas
- numpy
- matplotlib

---

## ▶️ How to Run
1. Open `notebook_1.ipynb` 
2. Upload datasets into:
3. Run all cells in order
4. Output charts will be saved in:
5. Merged dataset will be saved as:

---

## 📊 Key Insights (Summary)
- Trading activity (volume + trades) is slightly higher during **Fear** periods.
- Profitability (PnL) is highest during **Fear**, while **Extreme Fear** shows low profits.
- Win rate is highest in **Greed**, but higher win rate does not always mean higher profit.
- Average trade size increases during **Extreme Greed**, showing higher risk-taking.

---

## 📌 Outputs
The notebook generates the following charts:
- Sentiment vs Total Trading Volume
- Sentiment vs Total Daily PnL
- Win Rate by Sentiment Classification
- Average Trade Size by Sentiment Classification

---

## 👤 Author
**Harsh Kumar**

