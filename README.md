# Project: Cognitive Load Detection from EEG + GSR 

Objective: Classify task difficulty or NASA-TLX scores based on brainwave and GSR data.

ML Techniques: Feature engineering on Delta, Theta, Alpha bands + deep neural networks. 


## Structure

```
project/
├── data/                # Place your PSY.csv, EEG.csv, GSR.csv and outputs here
├── notebooks/           # Jupyter notebooks (01-05)
├── models/              # Saved model artifacts (xgb_model.pkl, cnn_lstm_model.pt)
└── README.md
```


## Notes

- The notebooks include templates and minimal example code — edit them to match your exact column names and project goals.
- `xgb_model.pkl` is a placeholder name; the code will use scikit-learn RandomForest if XGBoost is not installed. Replace with real XGBoost training in the notebook if needed.
- `cnn_lstm_model.pt` is a placeholder state_dict saved by the template if PyTorch is available.



- Python 3.8+
- pandas, numpy, scikit-learn, joblib
- scipy (for signal processing)
- xgboost (optional)
- torch (optional, for deep models)
