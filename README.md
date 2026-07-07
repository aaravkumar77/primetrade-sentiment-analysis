# Bitcoin Trader Performance vs Market Sentiment

Analysis of Hyperliquid trader data against the Bitcoin Fear & Greed Index, 
done as part of Primetrade.ai's data science hiring assignment.

## Datasets
- `Dataset/fear_greed_index.csv` — daily market sentiment (2018–2025)
- `Dataset/historical_data.csv` — Hyperliquid trader execution history (2023–2025)

## Approach
1. Cleaned and merged both datasets by date
2. Compared trader performance (PnL, win rate, position size, direction) across sentiment categories
3. Ran a Mann-Whitney U test to confirm findings were statistically significant
4. Visualized results with bar charts and a box plot

## Key Finding
Traders showed contrarian behavior — going long more during Fear and less 
during Greed — and this behavior was associated with higher win rates and 
profit during Fear periods (p = 1.30 × 10⁻⁶⁸, statistically significant).

## Files
- `Bitcoin_Sentiment_Analysis.ipynb` — full analysis notebook
- `Dataset/` — source CSVs
- Chart images (`.png`) generated from the notebook

## Strategy Implication
Market sentiment can act as a contrarian signal — consider increasing exposure 
during Fear and reducing it during Extreme Greed due to higher volatility of outcomes.