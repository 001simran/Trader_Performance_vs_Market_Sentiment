# trader-sentiment-analysis/

**Author:** Simranjit Kaur  
**Role:** Data Science Intern  

---

## Overview
This project analyzes how Bitcoin market sentiment (Fear/Greed) affects trader behavior and performance.  
We explore PnL, trade size, frequency, risk-adjusted returns, and behavioral patterns to derive actionable trading strategies.

---

## Problem Statement

Can market sentiment (Fear vs Greed) explain differences in trader performance and risk behavior?
This project investigates whether traders behave differently under varying sentiment regimes and whether these patterns can inform better trading strategies.

## Methodology

1. Merged historical trading data with daily Fear & Greed Index.
2. Categorized sentiment into:
   - Extreme Fear
   - Fear
   - Neutral
   - Greed
   - Extreme Greed
3. Calculated key performance metrics:
   - Average PnL
   - Trade Frequency
   - Position Size
   - Maximum Drawdown
   - Sharpe Ratio
4. Compared performance across sentiment regimes.

## Key Findings

- Traders take larger positions during Greed periods.
- Drawdowns increase significantly during Extreme Greed.
- Risk-adjusted returns (Sharpe Ratio) are higher during Fear phases.
- Trade frequency spikes during high emotional sentiment regimes.

## Strategy Recommendations

1. During Extreme Fear:
   - Reduce leverage.
   - Focus on selective long positions due to better risk-adjusted returns.

2. During Extreme Greed:
   - Reduce position size.
   - Tighten stop-loss levels due to higher drawdown risk.

These rules help traders adapt to emotional market cycles.

## Folder Structure

trader-sentiment-analysis/
│
├── data/                     # Input CSV files
│   ├── fear_greed_index.csv
│   └── historical_data.csv
│
├── notebook/                 # Jupyter notebook analysis
│   └── analysiss.ipynb
│
├── output/                   # Generated charts and result tables
│   ├── charts/
│   └── tables/
│
├── README.md
├── requirements.txt
└── .gitignore

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Jupyter Notebook

## How to Run

1. Clone the repository
2. Install dependencies:
   pip install -r requirements.txt
3. Open notebook/analysiss.ipynb
4. Run all cells to reproduce results
