# 📈 Geometric Brownian Motion: Simulation, Estimation, Pricing, and Hedging

This repository presents a **notebook-based quantitative finance project** that studies **Geometric Brownian Motion (GBM)** as a model for asset prices. The project connects **stochastic process theory** with **practical financial applications**, including simulation, parameter estimation from real market data, option pricing, and discrete-time delta hedging.

The primary goal is to examine **how well the continuous-time GBM framework performs in practice**, and to understand its limitations through empirical analysis and numerical experiments.

---

## 🔍 Project Objectives

- Simulate asset price dynamics under Geometric Brownian Motion
- Validate theoretical properties of GBM using Monte Carlo simulation
- Estimate drift and volatility parameters from real financial data
- Price European options using both analytical and simulation-based methods
- Analyse hedging performance and hedging error under discrete rebalancing

---

Each notebook is self-contained and builds on the results of the previous one, forming a coherent research-style workflow.

---

## 📘 Notebook Overview

### 00_intro_and_theory.ipynb
Introduces the Geometric Brownian Motion model, including its stochastic differential equation, closed-form solution, and key assumptions. The theoretical motivation and known limitations of GBM in modelling financial markets are also discussed.

### 01_gbm_simulation.ipynb
Implements Monte Carlo simulation of GBM price paths. The notebook validates theoretical properties such as the distribution of log-returns and the lognormality of terminal prices.

### 02_parameter_estimation.ipynb
Uses real market data (downloaded via Yahoo Finance) to estimate drift and volatility parameters. Maximum likelihood estimation and rolling volatility analysis are employed to compare empirical behaviour with GBM assumptions.

### 03_option_pricing.ipynb
Prices European call and put options using both the closed-form Black–Scholes formula and Monte Carlo simulation under a risk-neutral GBM framework. Convergence behaviour and variance reduction techniques are explored.

### 04_delta_hedging.ipynb
Simulates discrete-time delta hedging strategies and studies the resulting hedging error. The effects of rebalancing frequency, volatility misspecification, and model assumptions are analysed.

---

## 📊 Data Sources

- Daily adjusted closing prices obtained via the `yfinance` Python package (Yahoo Finance)
- Liquid equity indices or large-cap stocks (e.g. SPY)

No third-party datasets (e.g. Kaggle) are required.

---

## 🧰 Dependencies

The project is implemented entirely in Python using Jupyter notebooks. Key libraries include:

- numpy
- pandas
- scipy
- matplotlib
- yfinance

---

## 🎯 Intended Audience

This project is intended for:
- Students of statistics, mathematics, or engineering
- Individuals interested in quantitative finance or financial engineering
- Readers seeking an end-to-end illustration of stochastic modelling in finance

The notebooks assume basic familiarity with probability, calculus, and Python.

---

## 🚀 Future Extensions

Possible extensions include:
- Stochastic volatility models (e.g. Heston model)
- Jump-diffusion processes
- Transaction costs in hedging
- Empirical backtesting of hedging strategies
