# Bitcoin Investor

This repository showcases a Bitcoin trading algorithm I developed to explore the intersection of technical analysis and machine learning in cryptocurrency trading. Motivated by a deep interest in trading algorithms and the dynamic world of cryptocurrencies, this project aims to understand and innovate strategies for navigating volatile markets.

## Overview

My solution evolved through three key approaches, each building upon the lessons learned from the previous one:

### Golden Crossover Strategy  
The Golden Crossover Strategy used simple moving averages (SMAs) to generate buy and sell signals, offering a straightforward and computationally inexpensive approach. However, its reliance on lagging indicators made it susceptible to whipsaws and limited by a lack of robust risk management. This strategy highlighted the importance of incorporating confirmation signals and adaptability to improve trading outcomes.

### GARCH Model with MACD Signals  
The GARCH Model with MACD Signals combined volatility forecasting from the GARCH model with a MACD-based trend-following strategy, resulting in significantly improved returns (+800% over four years) and better risk management. Despite its effectiveness, the approach faced challenges from an over-reliance on trend continuation and assumptions of normality, particularly during market consolidation periods. This strategy underscored the importance of volatility-based risk management for more informed trading decisions.

### SMA + XGBoost Model  
The SMA + XGBoost Model integrated SMA-based signals with the XGBoost machine learning algorithm, achieving high predictive accuracy, strong feature engineering, and robust performance metrics, including Sharpe and Sortino ratios. While the approach required significant complexity and high-quality input data, it demonstrated the potential of machine learning to effectively handle complex market relationships and optimize trading strategies.

## Key Results

- **Cumulative Returns**: Modeled at $4,137,000 from an initial $100,000 investment (2018–2022).
- **Performance Metrics**: Consistent improvement in Sharpe and Sortino ratios across approaches.
- **Market Insights**: Highlighted the dynamic nature of volatility and the importance of robust risk management.

> **Note**: Results assume ideal conditions with no losses, focusing on percentage-based analysis for general applicability.
