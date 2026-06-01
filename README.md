# Trader Performance vs Market Sentiment Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance on Hyperliquid. The analysis combines the Bitcoin Fear & Greed Index with historical trader data to understand how market sentiment influences profitability, trading activity, and position sizing.

---

## Datasets Used

### Bitcoin Fear & Greed Index Dataset
Contains daily market sentiment classifications:
* Extreme Fear
* Fear
* Neutral
* Greed
* Extreme Greed

### Hyperliquid Historical Trader Dataset
Contains:
* Trade timestamps
* Trade size
* Trade direction (Long/Short)
* Profit and Loss (PnL)
* Trader account information

---

## Methodology

### Data Preparation
* Loaded both datasets using Pandas.
* Checked for missing values and duplicate records.
* Converted date and timestamp columns to datetime format.
* Merged datasets using the date column.

### Metrics Analyzed
* Daily Profit and Loss (PnL)
* Number of Trades per Day
* Average Trade Size
* Long/Short Ratio

### Trader Segmentation

#### Frequent vs Infrequent Traders
* 16 Frequent Traders
* 16 Infrequent Traders

#### Winners vs Non-Winners
* 29 Winners
* 3 Non-Winners

---

## Tools Used

* Python
* Pandas
* Matplotlib
* Google Colab

---

## How to Run

1. Open the notebook in Google Colab or Jupyter Notebook.
2. Upload the required datasets.
3. Install dependencies:

```bash
pip install pandas matplotlib
```

4. Run all cells in the notebook.
5. Review the generated charts and results.

---

## Key Insights

* Higher Profitability During Extreme Greed: Traders achieved the highest average profit during Extreme Greed periods. The average PnL during these periods was 67.89, which was higher than all other   sentiment categories. 
* Highest Trading Activity During Fear: Trading activity was highest during Fear periods. A total of 61,837 trades were recorded during Fear days, indicating increased market participation during uncertain market conditions.
-  Larger Position Sizes During Fear: The average trade size was highest during Fear periods at approximately $7,816. This suggests that traders were willing to take larger positions when the market was fearful.

---

## Strategy Recommendations

* Since average profitability was highest during Extreme Greed periods, traders may focus on high-conviction trading opportunities during these market conditions while maintaining proper risk management.
* Since trading activity and position sizes were highest during Fear periods, traders should consider using stricter risk management and smaller position sizes to reduce potential losses during volatile market conditions.
* Use the Fear & Greed Index alongside technical analysis.

---

## Conclusion

The analysis shows that market sentiment significantly influences trader behavior and performance. Understanding sentiment trends can help traders make better trading decisions and improve risk management strategies.
