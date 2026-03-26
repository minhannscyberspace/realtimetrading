#  Real-Time Trading with Deep Reinforcement Learning Agents

## Overview

This project explores the application of Deep Reinforcement Learning
(DRL) to algorithmic trading in a multi-asset portfolio setting. The
goal is to design agents that autonomously learn trading strategies
using historical price data and technical indicators, while optimizing
for risk-adjusted returns.

The system simulates trading over a portfolio of Dow Jones stocks,
evaluates multiple DRL algorithms, and integrates an ensemble agent and
a trading assistant chatbot.


## Key Features

-   Multi-asset portfolio trading (25 Dow Jones stocks)
-   PPO, A2C, DDPG, SAC, TD3 implementations
-   Ensemble agent
-   Technical indicators (MACD, RSI, CCI, ADX)
-   Optuna hyperparameter tuning
-   Financial evaluation metrics
-   Trading assistant chatbot

## Problem Formulation

State: - Market features + portfolio state

Action: - Continuous \[-1, 1\] per asset

Reward: reward = Δ(net worth) - transaction_cost

## Data

-   Source: Alpha Vantage
-   Train: 2014--2020
-   Validation: 2021
-   Test: 2022--2025
NOTE: stock data is not included due to size.

To reproduce:
- Use Alpha Vantage API

##  Evaluation

-   Net worth
-   Sharpe ratio
-   Volatility
-   Reward curve

## Future Work

-   LSTM / Transformer
-   CVaR risk modeling
-   Real-time deployment


## 🛠️ Installation

git clone https://github.com/minhannscyberspace/realtimetrading.git cd
realtimetrading pip install -r requirements.txt

## 👤 Author

Minh Nguyen
