# Cryptocurrency Price Forecasting using Hybrid Models

**Authors:** Raghav Raj Sah, Kaito Hikino, Pranjal Chalise

---

## Project Overview

We've built a comprehensive cryptocurrency price forecasting system that combines multiple machine learning approaches to predict Bitcoin's next-day closing price. Our system includes a baseline model, LSTM neural networks, ARIMA, XGBoost, and sentiment analysis components. The project features a complete pipeline from data preparation to model evaluation, with a focus on improving prediction accuracy through model ensembling.

---

## Project Structure

```
.
├── Code/                             # Core implementation notebooks
│   ├── baseline.ipynb                # Simple baseline model
│   ├── lstm_model.ipynb              # LSTM implementation
│   └── milestone_1_crypto-forecast.ipynb # Data preprocessing
│
├── Data/                             # Dataset storage (not tracked)
│
├── Presentations/                    # Project presentations
│
├── submission.ipynb                  # Final submission notebook
├── paper.pdf                        # Project paper
├── SentimentAnalysis.ipynb          # Sentiment analysis implementation
├── ARIMA,_XGBoost,_Updated_LTSM,_Baseline_and_HybridModel (1).ipynb # Advanced models
├── Abstract.pdf                     # Project abstract
├── README.md                        # This file
├── requirements.txt                 # Project dependencies
└── .gitignore                       # Git ignore rules
```

> **Note:** The `Data/` directory is excluded from version control to keep the repository size manageable.

---

## Getting Started

1. **Clone and setup:**
   ```bash
   git clone https://github.com/Khik2219/Cryptocurrency-Price-Forecasting-Using-Hybrid-Models.git
   pip install -r requirements.txt
   ```

2. **Data preparation:**
   - Run `Code/milestone_1_crypto-forecast.ipynb` to process the data

3. **Model training:**
   - Start with `Code/baseline.ipynb` for the simple model
   - Try `Code/lstm_model.ipynb` for the LSTM implementation
   - Explore `ARIMA,_XGBoost,_Updated_LTSM,_Baseline_and_HybridModel (1).ipynb` for advanced models
   - Check out `SentimentAnalysis.ipynb` for sentiment-based predictions

4. **Final results:**
   - See `submission.ipynb` for the complete implementation and results
   - Read `paper.pdf` for detailed methodology and findings

---

## What's Inside

- **Data Processing** (`milestone_1_crypto-forecast.ipynb`): Handles data cleaning, feature engineering, and train/test splitting
- **Baseline Model** (`baseline.ipynb`): Implements a simple "tomorrow equals today" prediction
- **LSTM Model** (`lstm_model.ipynb`): Deep learning approach using 30-day sequences
- **Advanced Models** (`ARIMA,_XGBoost,_Updated_LTSM,_Baseline_and_HybridModel (1).ipynb`): Combines multiple models for better predictions
- **Sentiment Analysis** (`SentimentAnalysis.ipynb`): Integrates social media sentiment data
- **Final Implementation** (`submission.ipynb`): Complete solution with all components

---

## Key Features

- Multiple model approaches (LSTM, ARIMA, XGBoost)
- Sentiment analysis integration
- Model ensembling
- Comprehensive evaluation metrics
- Clean, modular code structure

---

## Notes

- The `Data/` directory is excluded from git to keep the repository size manageable
- External datasets should be cited according to their original sources
- All code is well-documented with clear explanations

---

## License

This project is for academic purposes. External code and data are subject to their respective licenses.

---

## Contact

Feel free to reach out through GitHub for questions or collaboration.

---

**GitHub Repository:** [https://github.com/Khik2219/Cryptocurrency-Price-Forecasting-Using-Hybrid-Models.git]

---

