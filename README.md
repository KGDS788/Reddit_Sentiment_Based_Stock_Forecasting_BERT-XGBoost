# Sentiment-Based Stock Price Prediction Using Transformer Models

This repository contains my MSc dissertation project titled "Harnessing the Power of Transformer Architectures for Sentiment-Based Stock Market Prediction", submitted to the University of Exeter.

## Overview

This research investigates the effectiveness of BERT-based models in predicting stock price movements using sentiment analysis from Reddit posts. The project evaluates how combining NLP-driven sentiment with financial time series data can enhance stock prediction accuracy, particularly for Apple Inc. (AAPL).

## Objectives

- Analyze Reddit sentiment using BERT.
- Correlate sentiment with historical AAPL stock data.
- Compare BERT performance with traditional ML models.
- Improve prediction accuracy using an ensemble with XGBoost.

## Key Features

- Sentiment classification of Reddit posts (`apple`, `wallstreetbets`, etc.).
- Financial data extraction from Yahoo Finance via `yfinance`.
- Data cleaning, feature engineering, and SMOTE-based class balancing.
- Sentiment model built using `bert-base-uncased`.
- Hyperparameter tuning using Optuna.
- Ensemble learning with BERT + XGBoost.
- Achieved 81.85% sentiment classification accuracy.

## Files Included

- `Report.pdf` — Full dissertation report
- `README.md` — This file

## Results

- Sentiment accuracy: 81.85% (after threshold optimization)
- Stock sentiment correlation:
  - Long-term: 0.7564
  - Lagged (next-day): 0.7704
- Ensemble improvement: +0.92% accuracy over BERT-only

## Technologies Used

- Python, Pandas, NumPy
- HuggingFace Transformers (`bert-base-uncased`)
- scikit-learn, Optuna, SMOTE
- XGBoost, yfinance, PRAW
- Matplotlib, Seaborn

## Visual Insights

- ROC and Precision-Recall curves for all sentiment classes
- Short vs long-term sentiment-price trends
- Daily sentiment trend charts

## Author

Kshitiz Gautam 
MSc Data Science, University of Exeter  
kshitiz937@gmail.com

## Citation

If you reference or use any ideas from this work, please cite it as:

Gautam, K. (2024).Harnessing the Power of Transformer Architectures for Sentiment-Based Stock Market Prediction. https://github.com/KGDS788.github.io/Reddit_Sentiment_Based_Stock_Forecasting_BERT_XGBoost


## Disclaimer

This project was conducted for academic purposes. No financial decisions should be made based solely on this model or analysis.
