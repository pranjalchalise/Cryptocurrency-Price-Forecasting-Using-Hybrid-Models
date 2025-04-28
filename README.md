# Hybrid Crypto‑Price Forecasting

We try to predict the next‑day Bitcoin closing price by mixing a few different models and comparing them.

---

## Project summary (very short)
1. Clean the raw Bitcoin price data (daily OHLC from Binance / Kaggle).
2. Build a super‑simple baseline that says “tomorrow = today.”
3. Train a small LSTM network that looks at the last 30 days to guess tomorrow.
4. Compare the errors.  Later milestones will add ARIMA, XGBoost and sentiment.

Right now we have the full **load → train → evaluate** pipeline working (Milestone 2).

---

## Milestones
| Milestone | What we finished | Main files |
|-----------|------------------|------------|
| **M1 – Data prep** | cleaning, feature engineering, train/test split | `milestone1.py` |
| **M2 – Baseline + LSTM** | naive baseline, LSTM model, evaluation script | `baseline.py`, `lstm_model.py`, |

---

## Folder layout
```
.
├── baseline_naive.py     # simple "tomorrow = today" benchmark
├── lstm_model.py         # trains LSTM and saves predictions
├── requirements.txt      # pip install -r requirements.txt
└── README.md             # this file
```

---

## Quick start (Milestone 2)
```bash
# clone the repo and install packages
pip install -r requirements.txt

# 1) prep the data\python data_prep.py

# 2) run the baseline
python baseline_naive.py

# 3) train the LSTM
python lstm_model.py --epochs 10 --seq_len 30

# 4) evaluate both models
python evaluate.py
```
If everything runs you’ll see numbers something like:
```
Baseline  RMSE: 0.05
LSTM      RMSE: 0.028
```
(Values are in the 0‑1 scaled space.)

---

## What each script does
* **milestone1.py** – loads the raw CSV, fixes missing rows, removes outliers, adds moving averages, RSI, daily return, then saves train / test csv files.
* **baseline.py** – reads the processed data and predicts tomorrow’s close equals today’s close.
* **lstm_model.py** – builds a small LSTM with 64 units and dropout, trains on 30‑day sequences, and writes its predictions.

---


## Planned next steps
* pull Twitter / Reddit sentiment (CrypTop12 dataset)
* add ARIMA and XGBoost models
* create an ensemble that averages or weights the three models
* tune hyper‑parameters with a small grid search

---


