# AI Finance Prediction Pipeline

## Overview
This project contains a machine learning pipeline for predicting cryptocurrency and stock prices. It includes data preprocessing, model training, prediction, and visualization. The main goal is to provide a reusable, easy-to-follow notebook for financial time series prediction.

---

## Repository Structure

ai_finance_project/
│
├── data/ # Raw and processed datasets
│ ├── BTC.csv
│ ├── ETH.csv
│ ├── LTC.csv
│ ├── XPR.csv
│ ├── crypto_combine.csv
│ ├── economic_indicators.csv
│ ├── stock_prices.csv
│ ├── test.csv
│ └── train.csv
│
├── finance_pipeline.ipynb # Main Jupyter notebook
├── processed_crypto_data.csv # Processed datasets
├── crypto_price_predictor.pkl# Trained model (pickle)
├── xgb_crypto_model.json # Model configuration
├── xgb_crypto_model.pkl # XGBoost model
├── setup_ai_env.zsh # Setup script for environment
├── LICENSE # MIT License
└── .gitignore # Files/folders excluded from git


---

## Installation & Setup

1. Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/ai_finance_project.git
cd ai_finance_project

python3 -m venv ai_project_env
source ai_project_env/bin/activate

pip install -r requirements.txt

If requirements.txt does not exist, install common packages: 

pip install pandas numpy matplotlib scikit-learn xgboost scipy jupyter

jupyter notebook

Open finance_pipeline.ipynb and follow the cells.

Usage

-Load your training and test datasets from data/.

-Run preprocessing, feature creation, and model training in sequence.

-Visualize predictions, actuals, and smoothed outputs.

-Metrics such as MSE, MAE, and R² are calculated automatically.

-Note: “Actual” graphs may appear jagged due to data characteristics.

Notes & Known Issues

-Date columns may vary between datasets; code includes flexible parsing.

-Predictions are smoothed using Gaussian filters.

-R² may appear negative for small or noisy datasets — MSE and MAE are more reliable indicators.

License

MIT License © 2025 Fatlum Dili

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software.


---



