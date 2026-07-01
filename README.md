# primetrade
# Trader Behaviour vs Bitcoin Market Sentiment

Data Science internship assignment (Primetrade.ai). Exploring whether trader
performance on Hyperliquid is linked to the Bitcoin Fear/Greed sentiment on
that day.

## Files
- `Trader_Behaviour_vs_Sentiment.ipynb` - main analysis notebook (all code + charts + insights)
- `fear_greed_index.csv` - daily sentiment classification (Fear, Greed, etc.)
- `historical_data.csv` - trade-level data (~211k rows). 

## How to run
```bash
pip install -r requirements.txt
jupyter notebook Trader_Behaviour_vs_Sentiment.ipynb
```

## What's inside
1. Load & merge trade data with daily sentiment
2. Win rate / avg PnL by sentiment
3. Buy-side order share by sentiment (herd vs contrarian check)
4. Top 20% vs bottom 20% traders - how each group reacts to sentiment
5. Coin preference shift between Extreme Fear and Extreme Greed
6. Correlation between sentiment score and daily PnL

## Key takeaways
- Traders perform best (highest win rate & avg PnL) on **Extreme Greed** days,
  worst on **Extreme Fear** days.
- Order flow is only mildly contrarian and that tilt doesn't pay off during fear.
- Top-performing accounts keep a consistent win-rate edge over weaker accounts
  across every sentiment regime, and the gap widens most during Extreme Greed.
- Coin preference shifts with sentiment; BTC/ETH/SOL stay popular regardless.
- Raw sentiment score alone has weak linear correlation with daily PnL - the
  sentiment *category* matters more than the *score*.

Full details and charts are in the notebook.
