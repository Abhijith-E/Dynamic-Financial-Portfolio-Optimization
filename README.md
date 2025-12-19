📈 Dynamic Financial Portfolio Optimization using TCN and CVaR

This repository contains my research work on AI-driven financial portfolio optimization using Temporal Convolutional Networks (TCNs) combined with Conditional Value-at-Risk (CVaR) minimization.
In this work, I focus on real-time financial data analysis, robust risk management, and adaptive portfolio allocation under volatile market conditions.

📄 Research Overview

Title: Dynamic Financial Portfolio Optimization Using Temporal Convolutional Networks and Real-Time Data Analysis
Author: Abhijith E
Affiliation: Department of Computer Science, CHRIST (Deemed to be University), Bengaluru, India

In this research, I propose an integrated framework that combines deep learning–based temporal modeling with statistical risk optimization techniques to overcome the limitations of traditional portfolio management methods.

🚀 Key Contributions

Temporal Convolutional Networks (TCNs)

I use dilated causal convolutions to capture both short-term and long-term dependencies in financial time-series data

The model preserves temporal causality, making it suitable for real-time forecasting

Enables efficient parallel computation compared to recurrent models

CVaR-Based Portfolio Optimization

I formulate portfolio allocation as a CVaR minimization problem to explicitly control tail risk

This approach provides more stable and risk-aware portfolios compared to variance-based methods

Hybrid Covariance Estimation

I apply Ledoit–Wolf shrinkage to reduce estimation noise

Eigenvalue regularization is used to ensure numerical stability and positive semi-definiteness

Automated Real-Time Data Pipeline

I design a volatility-adjusted feature engineering pipeline

Walk-forward validation is employed to adapt to changing market regimes

Robust technical indicators are used to ensure numerical stability

🧠 Methodology
1️⃣ Data Processing

I collect real-time market data using the Yahoo Finance API

Exponential smoothing is applied to reduce noise

Returns are normalized using volatility-adjusted scaling

A numerically stable formulation of RSI is used to avoid division errors

2️⃣ Feature Engineering

Average True Range (ATR) for volatility estimation

Chaikin Money Flow (CMF) for volume-based market pressure

Volatility-scaled technical indicators to adapt to market conditions

3️⃣ Temporal Modeling

I implement a multi-layer Temporal Convolutional Network consisting of:

Dilated causal convolutions

Batch normalization

ReLU activation

Dropout regularization

Global average pooling for temporal summarization

4️⃣ Portfolio Optimization

Portfolio weights are obtained by minimizing CVaR with L2 regularization

Asset weight constraints are enforced for realistic allocations

Shrinkage-based covariance estimation improves risk estimation robustness

📊 Experimental Results

Backtesting Period: 2018 – 2023
Benchmark: S&P 500

Metric	My Model	S&P 500
Annual Return	18.7%	9.2%
Sharpe Ratio	0.84	0.52
Sortino Ratio	1.27	0.68
Max Drawdown	-22.4%	-33.9%

These results demonstrate that my approach achieves higher risk-adjusted returns, lower downside risk, and better capital preservation compared to the benchmark.

📈 Optimized Portfolio Allocation

The optimized portfolio obtained from my CVaR-based framework shows a diversified asset allocation:

TLT: 23.5%

GLD: 22.1%

SPY: 14.8%

VTI: 14.4%

IWM: 12.9%

QQQ: 12.3%

This allocation balances growth, stability, and downside protection, aligning with the goal of maximizing risk-adjusted returns.

🛠️ Technologies Used

Python

PyTorch

NumPy

Pandas

SciPy

yFinance

Matplotlib

🔮 Future Work

In future extensions of this research, I plan to:

Integrate news and sentiment analysis

Explore reinforcement learning for dynamic portfolio rebalancing

Investigate quantum-inspired optimization techniques

Incorporate multi-modal financial data for improved prediction accuracy

📌 Citation

If you use or build upon this work, please cite:

Abhijith E,
"Dynamic Financial Portfolio Optimization Using Temporal Convolutional Networks and Real-Time Data Analysis",
Department of Computer Science, CHRIST (Deemed to be University), Bengaluru.

👤 Author

Abhijith E
M.Sc. Artificial Intelligence and Machine Learning
CHRIST (Deemed to be University), Bengaluru
📧 abhijith.e@msam.christuniversity.in
