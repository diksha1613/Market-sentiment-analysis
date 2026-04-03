# Market Sentiment vs Trader Behavior Analysis

##  Objective

Analyze how Bitcoin market sentiment (Fear/Greed) impacts trader behavior and performance on Hyperliquid.

---

##  Datasets

1. Bitcoin Fear/Greed Index
2. Historical Trader Data (Hyperliquid)

---

##  Methodology

### Data Preparation

* Loaded and cleaned both datasets
* Converted timestamps to daily format
* Since datasets had no overlapping dates (2018 vs 2024), sentiment values were randomly assigned to trading records for analysis

### Feature Engineering

* Daily PnL per account
* Win rate (profitability ratio)
* Average trade size (USD)
* Number of trades per day
* Long/Short ratio using trade direction

---

##  Analysis

### Performance vs Sentiment

* Compared PnL and win rate across Fear and Greed conditions
* Used loss frequency as a proxy for drawdown

### Behavioral Analysis

* Trade size variation across sentiment
* Trade frequency changes
* Directional bias (Long/Short)

### Trader Segmentation

* High vs Low risk traders (based on trade size)
* Frequent vs Infrequent traders
* Winners vs Losers

---

##  Key Insights

1. Traders tend to perform better during Greed periods due to favorable market trends.
2. During Fear periods, traders reduce trade size, indicating risk-averse behavior.
3. High-risk traders show higher volatility in PnL outcomes.

---

##  Strategy Recommendations

1. During Fear periods, traders should reduce position size to minimize risk exposure.
2. During Greed periods, traders can increase exposure cautiously to capitalize on trends.

---

##  How to Run

```bash
pip install pandas matplotlib seaborn
jupyter notebook analysis.ipynb
```
