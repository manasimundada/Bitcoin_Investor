# Bitcoin Investor

This repository showcases the different Bitcoin trading algorithms I developed to explore the intersection of technical analysis and machine learning in cryptocurrency trading. Motivated by a deep interest in trading algorithms and the dynamic world of cryptocurrencies, this project aims to understand and innovate strategies for navigating volatile markets.

## Overview

My solution evolved through three key approaches, each building upon the lessons learned from the previous one:

### Golden Crossover Strategy  
The Golden Crossover Strategy used simple moving averages (SMAs; 12 ans 45 days) to generate buy and sell signals, offering a straightforward and computationally inexpensive approach. However, its reliance on lagging indicators made it susceptible to whipsaws and limited by a lack of robust risk management. This strategy highlighted the importance of incorporating confirmation signals and adaptability to improve trading outcomes. I did try implementing an ATR-based stoploss but was simply met with lower profits.

### GARCH Model with MACD Signals  
The GARCH Model with MACD Signals combined volatility forecasting from the GARCH model with a MACD-based trend-following strategy, resulting in significantly improved returns (+800% over four years) and better risk management. Despite its effectiveness, the approach faced challenges from an over-reliance on trend continuation and assumptions of normality, particularly during market consolidation periods. This strategy underscored the importance of volatility-based risk management for more informed trading decisions.

### XGBoost Model with RSI  
The final model employed an XGBoost classifier using the Relative Strength Index (RSI) as the sole input feature to predict buy, sell, and hold signals. RSI, calculated over a 14-day period, was imputed for missing values using `SimpleImputer` to ensure data consistency. Backtesting the strategy against BTC's daily returns demonstrated superior cumulative returns, Sharpe and Sortino ratios, and reduced drawdown compared to a buy-and-hold approach. The hyperparameters were, admittedly, brute-force-optimized for maximum net profit.

## Key Results

- **Cumulative Returns**: Modeled at $63,663,029 from an initial $100,000 investment (2018–2022).
- **Performance Metrics**: Consistent improvement in Sharpe and Sortino ratios across approaches.
- **Market Insights**: Highlighted the dynamic nature of volatility and the importance of robust risk management.
