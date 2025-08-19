📊 Gold Regime Analysis with Machine Learning & Deep Learning

This repository explores how machine learning (ML), deep learning (DL), and regime detection can be applied to gold price forecasting and strategy design.

⚠️ Disclaimer: This project is for research and educational purposes only. It is not investment advice.

🌐 Project Overview

Financial markets do not move in a straight line — they transition through regimes:

Risk-On → markets rally, gold often trends positively.

Risk-Off → uncertainty rises, gold volatility increases.

Crisis → extreme stress periods where gold may spike, but then corrects.

By combining regime detection with predictive ML/DL models, this project aims to design more robust gold trading strategies.

⚙️ Methodology
1. Data & Features

Assets: Gold (GC=F), macroeconomic indicators, dollar index, yields, equities, commodities.

Feature engineering:

Rolling statistics & lags

Technical indicators (RSI, MACD, momentum, volatility)

Macro spreads and correlations

2. Models

Machine Learning:

Logistic Regression (baseline)

XGBoost (tree-based ML)

Deep Learning:

LSTM (captures sequential/temporal dependencies in gold)

Regime Detection:

Hidden Markov Models (HMM) with 3 regimes (Risk-On, Risk-Off, Crisis)

Hybrid Strategies:

Model signals gated by favorable regimes (e.g., only active during Risk-On).

3. Backtesting

Long/Flat and Long/Short strategies

Performance metrics: CAGR, Volatility, Sharpe Ratio, Max Drawdown, Turnover

Transaction costs included (bps).

🔑 Key Findings

Short-term:

Machine learning (XGB, LogReg) captures quick moves but struggles in crises.

Long-term:

Deep learning (LSTM) outperforms with higher Sharpe ratios, lower drawdowns, and more stable returns.

Hybrid approach:

Regime-gated LSTM further improves stability and reduces drawdowns by trading only in favorable conditions.

👉 Summary:

ML is better for short-term trading.

DL (LSTM) is better for long-term gold investment strategies.

Regime detection makes both approaches more resilient.

🚀 Next Steps

Future extensions include:

Cointegration analysis (Johansen test) to capture long-term structural relationships between gold and macro assets.

Kalman filtering & VECM for dynamic relationships.

Explainability tools (e.g., SHAP) for ML models.

Comparison with alternative assets (Silver, Crude Oil, USD, Treasuries).

📈 Sample Results
Feature Selection

Equity Curves (ML Baselines)

LSTM Strategies

Hybrid Regime-Gated Strategies

🛠️ Tech Stack

Python (Pandas, NumPy, Scikit-learn, XGBoost, TensorFlow/Keras)

Statsmodels (HMM, cointegration)

Matplotlib/Seaborn (visualization)