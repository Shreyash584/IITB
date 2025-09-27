# Project: Cognitive Load Detection from EEG + GSR 

Objective: Classify task difficulty or NASA-TLX scores based on brainwave and GSR data.\

ML Techniques: Feature engineering on Delta, Theta, Alpha bands + deep neural networks. 


## Structure

```
project/
├── data/                # Place your PSY.csv, EEG.csv, GSR.csv and outputs here
├── notebooks/           # Jupyter notebooks (01-05)
├── models/              # Saved model artifacts (xgb_model.pkl, cnn_lstm_model.pt)
└── README.md
```

## How to use

1. Put your CSVs into `project/data/` as `PSY.csv`, `EEG.csv`, `GSR.csv`.
2. Open `project/notebooks/01_preprocessing.ipynb` and run cells to clean and align data.
3. Run `02_feature_engineering.ipynb` to produce `data/features.csv`.
4. Run `03_modeling_baseline_classification.ipynb` to train a baseline model (saved to `models/xgb_model.pkl`).
5. Optionally run `04_modeling_deep_timeseries.ipynb` to train a CNN-LSTM (requires PyTorch).
6. Use `05_analysis.ipynb` for evaluation and plots.

## Notes

- The notebooks include templates and minimal example code — edit them to match your exact column names and project goals.
- `xgb_model.pkl` is a placeholder name; the code will use scikit-learn RandomForest if XGBoost is not installed. Replace with real XGBoost training in the notebook if needed.
- `cnn_lstm_model.pt` is a placeholder state_dict saved by the template if PyTorch is available.

## Requirements (suggested)

- Python 3.8+
- pandas, numpy, scikit-learn, joblib
- scipy (for signal processing)
- xgboost (optional)
- torch (optional, for deep models)
