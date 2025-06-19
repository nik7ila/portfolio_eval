# portfolio_eval
# 📊 Portfolio Evaluation Project

This notebook analyzes a portfolio of four stocks (`AAPL`, `TSLA`, `DIS`, `AMZN`) with equal weights, comparing its performance to the S&P 500 benchmark from 2015 to 2025.

## 📁 Contents
- Data loading using `yfinance`
- Daily & cumulative returns
- Portfolio vs S&P 500 performance
- Performance metrics via `quantstats`
- Sharpe & Sortino ratio visualizations
- Year-end return comparison

## 📈 Highlights
End-of-Year Returns:
       Portfolio   S&P 500
Date                     
2015   0.309356 -0.006928
2016   0.050798  0.095350
2017   0.394963  0.194200
2018   0.117067 -0.062373
2019   0.447829  0.288781
2020   1.616504  0.162589
2021   0.192059  0.268927
2022  -0.459651 -0.194428
2023   0.595231  0.242305
2024   0.461970  0.233090

Benchmark    Strategy
------------------  -----------  ----------
Start Period        2015-01-05   2015-01-05
End Period          2024-12-31   2024-12-31
Risk-Free Rate      0.0%         0.0%
Time in Market      100.0%       100.0%

Cumulative Return   185.77%      1,120.09%
CAGR﹪              7.52%        18.86%

Sharpe              0.68         1.05
Prob. Sharpe Ratio  98.29%       99.95%
Sortino             0.95         1.52
Sortino/√2          0.67         1.08
Omega               1.2          1.2

Max Drawdown        -33.92%      -50.72%
Longest DD Days     745          1037

Gain/Pain Ratio     0.14         0.2
Gain/Pain (1M)      0.8          1.29

Payoff Ratio        0.92         0.95
Profit Factor       1.14         1.2
Common Sense Ratio  1.06         1.24
CPC Index           0.56         0.63
Tail Ratio          0.93         1.03
Outlier Win Ratio   5.03         3.0
Outlier Loss Ratio  5.25         3.1

MTD                 -2.5%        5.85%
3M                  2.5%         25.37%
6M                  7.71%        36.42%
YTD                 23.31%       46.2%
1Y                  23.31%       46.2%
3Y (ann.)           6.93%        8.82%
5Y (ann.)           8.52%        19.06%
10Y (ann.)          7.52%        18.86%
All-time (ann.)     7.52%        18.86%

Avg. Drawdown       -1.72%       -3.89%
Avg. Drawdown Days  20           32
Recovery Factor     3.57         5.67
Ulcer Index         0.08         0.15
Serenity Index      1.2          1.24

- **Cumulative Return** (Portfolio): 1120%
- **CAGR**: 18.86%
- **Sharpe Ratio**: 1.05
- **Max Drawdown**: -50.72%
- **Sortino Ratio**: 1.52

## 📊 Visualizations
- Cumulative returns plot
![cumulative returns](cum_returns.png)
- Sharpe vs Sortino ratio bar chart
![sharpe sortino](sharpe_sortino.png)
- portfolio summary plot
![portfolio summary](port_summary.png)


## 📎 Dependencies
```bash
pip install yfinance quantstats matplotlib seaborn
