# Pairs Trading Frequency Analysis

A comprehensive study investigating how trading frequency affects pairs trading performance in the U.S. equity market.

## Overview

This project implements a classic pairs trading strategy using rolling hedge ratios and z-score thresholds to analyze the impact of different trading frequencies (hourly, daily, weekly) on strategy performance. The analysis covers 2,333 pairs selected from S&P 500 stocks.

## Methodology

1. **Pair Selection**: Systematic screening of S&P 500 combinations using correlation and cointegration tests
2. **Strategy Implementation**: Rolling beta calculation with GPU acceleration for computational efficiency
3. **Signal Generation**: Z-score based entry/exit thresholds with holding period limits and stop-loss mechanisms
4. **Performance Analysis**: Comprehensive backtesting across three frequencies with consistent parameters

## Technical Stack

- **Platform**: Jupyter Notebook (Google Colab)
- **Data Sources**: Alpaca Markets API
- **GPU Computing**: CUDA-accelerated statistical analysis using CuPy and cuDF
- **Analysis Tools**: Python (pandas, numpy, statsmodels, matplotlib, seaborn)

## Key Findings

- **Risk-Adjusted Performance**: Hourly trading demonstrated the best risk-adjusted returns, while daily trading performed worst
- **Risk Profile**: Higher-frequency strategies showed more consistent performance with better risk control
- **Return Analysis**: Only hourly strategies achieved positive average returns with superior downside protection
- **Drawdown Management**: Hourly strategies exhibited the least severe and most consistent drawdowns

## Repository Contents

- `pair_trading_final_project.ipynb` - Complete analysis with implementation, backtesting, and results
- `pair_trading_final_project.pdf` - Formatted report version of the analysis
- Comprehensive visualizations and statistical analysis
- GPU-optimized cointegration testing and rolling regression functions
