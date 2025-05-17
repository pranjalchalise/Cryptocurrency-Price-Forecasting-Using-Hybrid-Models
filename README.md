# Cryptocurrency Price Forecasting using Hybrid Models

**Authors:** Raghav Raj Sah, Kaito Hikino, Pranjal Chalise

---

## Project Overview

This project aims to forecast the next-day closing price of Bitcoin using a combination of machine learning and deep learning models. We compare the performance of a simple baseline, an LSTM neural network, and plan to integrate ARIMA, XGBoost, and sentiment analysis for a hybrid approach. The goal is to build a robust pipeline for data preparation, model training, and evaluation, ultimately improving prediction accuracy through model ensembling.

---

## Folder Structure

```
.
├── Code/
│   ├── baseline.ipynb                # Baseline "tomorrow = today" benchmark
│   ├── lstm_model.ipynb              # LSTM model training and prediction
│   └── milestone_1_crypto-forecast.ipynb # Data cleaning, feature engineering, train/test split
│
├── Data/                             # (Not tracked) Raw and processed datasets
│
├── Presentations/                    # Project presentations and slides
│
├── ARIMA,_XGBoost,_Updated_LTSM,_Baseline_and_HybridModel (1).ipynb # Hybrid and advanced models
├── SentimentAnalysis.ipynb           # Sentiment analysis integration
├── Abstract.pdf                      # Project abstract
├── README.md                         # Project documentation
├── requirements.txt                  # Python dependencies
├── .gitignore                        # Excludes raw data and large files
```

> **Note:** The `Data/` folder is excluded via `.gitignore` to avoid uploading large/raw datasets.

---

## Setup & Run Instructions

1. **Clone the repository and install dependencies:**
   ```bash
   git clone <https://github.com/Khik2219/Cryptocurrency-Price-Forecasting-Using-Hybrid-Models.git>
   pip install -r requirements.txt
   ```

2. **Prepare the data:**
   - Open and run all cells in `Code/milestone_1_crypto-forecast.ipynb`.

3. **Run the baseline model:**
   - Open and run all cells in `Code/baseline.ipynb`.

4. **Train the LSTM model:**
   - Open and run all cells in `Code/lstm_model.ipynb`.

5. **Run advanced/hybrid models:**
   - Open and run all cells in `ARIMA,_XGBoost,_Updated_LTSM,_Baseline_and_HybridModel (1).ipynb`.

6. **Sentiment analysis (optional/advanced):**
   - Open and run all cells in `SentimentAnalysis.ipynb`.

**Expected Output Example:**
```
Baseline  RMSE: 0.05
LSTM      RMSE: 0.028
```
*(Values are in the 0–1 scaled space.)*

---

## What Each Script/Notebook Does

- **Code/milestone_1_crypto-forecast.ipynb** – Loads raw data, cleans it, performs feature engineering, and splits into train/test sets.
- **Code/baseline.ipynb** – Implements a naive baseline: predicts tomorrow’s close equals today’s close.
- **Code/lstm_model.ipynb** – Builds and trains an LSTM model on 30-day sequences, outputs predictions.
- **ARIMA,_XGBoost,_Updated_LTSM,_Baseline_and_HybridModel (1).ipynb** – Implements ARIMA, XGBoost, updated LSTM, baseline, and hybrid/ensemble models.
- **SentimentAnalysis.ipynb** – Integrates sentiment data from social media for improved forecasting.

---

## Planned Next Steps

- Integrate Twitter/Reddit sentiment (CrypTop12 dataset)
- Add ARIMA and XGBoost models
- Create an ensemble (hybrid) model
- Tune hyperparameters with grid search

---

## Additional Notes

- **.gitignore:** Raw data and large files (e.g., `Data/`, `.csv`) are excluded from version control.
- **Licensing/Citation:** If using external datasets (e.g., Binance, Kaggle, CrypTop12), please cite the original sources as per their terms. For any external code, see comments in the relevant notebooks for attribution.
- **File Naming:** All scripts and notebooks use clear, descriptive names for easy navigation.

---

## License

This project is for academic purposes. For any external code or data, please refer to their respective licenses.

---

## Contact

For questions or collaboration, please contact us via GitHub.

---

**GitHub Repository:** [https://github.com/Khik2219/Cryptocurrency-Price-Forecasting-Using-Hybrid-Models.git]

---

