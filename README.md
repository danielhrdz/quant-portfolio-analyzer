# Quantitative Portfolio Analyzer

A Python-based portfolio analysis project that evaluates historical stock performance, portfolio risk, diversification, and risk-adjusted returns using real market data.

## Overview

This project analyzes a five-stock portfolio using historical market data from 2021 through 2025. The goal is to explore how diversification and asset allocation affect portfolio risk and return.

The project compares an equal-weight portfolio against the S&P 500 and uses Monte Carlo simulation to analyze thousands of possible portfolio allocations.

## Portfolio Assets

- Apple (AAPL)
- Microsoft (MSFT)
- NVIDIA (NVDA)
- JPMorgan Chase (JPM)
- Exxon Mobil (XOM)

These companies represent multiple sectors, allowing the analysis to examine the effects of diversification.

## Features

- Downloads historical market data using `yfinance`
- Calculates daily and annualized returns
- Measures annualized volatility
- Calculates Sharpe ratios
- Measures maximum drawdown
- Analyzes correlations between assets
- Simulates 10,000 portfolio allocations using Monte Carlo simulation
- Identifies simulated maximum-Sharpe and minimum-volatility portfolios
- Compares an equal-weight portfolio against the S&P 500 (SPY)
- Calculates compound annual growth rate (CAGR)
- Visualizes portfolio growth, drawdowns, correlations, and risk-return tradeoffs

## Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- yfinance
- Jupyter Notebook

## Key Results

Using historical data from 2021 through 2025:

- A $10,000 equal-weight portfolio grew to approximately $43,000.
- The portfolio achieved approximately 34.3% CAGR compared with 14.7% for SPY.
- Annualized portfolio volatility was approximately 25.1%, compared with 17.1% for SPY.
- Maximum portfolio drawdown was approximately -26.4%.
- The portfolio produced a historical Sharpe ratio of approximately 1.33 using an assumed 4% risk-free rate.
- Monte Carlo simulation demonstrated the tradeoff between portfolio risk and expected return across 10,000 different allocations.

## Methodology

Historical adjusted closing prices are used to calculate daily returns. These returns are then used to estimate annualized return, volatility, covariance, correlation, and risk-adjusted performance.

An equal-weight portfolio provides a baseline allocation. Monte Carlo simulation then generates 10,000 random portfolio weight combinations to explore the risk-return space and identify simulated maximum-Sharpe and minimum-volatility portfolios.

The equal-weight portfolio is also benchmarked against SPY to compare historical growth and risk characteristics.

## Limitations

This project is an educational analysis based on historical data and does not predict future investment performance.

The selected stocks were not chosen through an out-of-sample investment strategy, so historical performance relative to the S&P 500 should not be interpreted as evidence of future market outperformance.

Transaction costs, taxes, changing interest rates, and other real-world factors are not included.

## Project Notebook

The complete analysis, calculations, and visualizations are available in:

`portfolio_analysis.ipynb`

## Author

Daniel Hernandez  
Computer Engineering — University of North Texas
