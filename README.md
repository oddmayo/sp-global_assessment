# Stock Price Prediction — S&P Global Assessment

Predict next-day stock prices using historical price data and market news sentiment across 7 technology tickers.

## Directory Structure

```
.
├── 01_eda.ipynb                    # Data exploration & correlation analysis
├── 02_baseline_model.ipynb         # Baseline models (Ridge & XGBoost)
├── 03_news_enhanced_model.ipynb    # News enhanced models (VADER & FinBERT)
├── sources.ipynb                   # Used sources
├── requirements.txt                # Dependency specification
├── data/                           # Input datasets
│   ├── news.csv
│   └── price.csv
└── output/                         # Processed features & baseline results
    ├── baseline_results.csv
    └── price_features.csv
```

## Setup

1. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

2. **Execution Order**:
   - Run `01_eda.ipynb` for initial data exploration.
   - Run `02_baseline_model.ipynb` to generate `output/price_features.csv` and train baseline models.
   - Run `03_news_enhanced_model.ipynb` to compute news sentiment features (VADER + FinBERT) and evaluate the full model matrix.
```