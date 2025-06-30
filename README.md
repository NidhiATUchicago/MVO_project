📈 Mean-Variance Optimization Analysis

This repository contains code and write-up for the Mean-Variance Optimization exercise, completed as part of our financial analysis coursework. The project utilizes historical ETF return data to analyze and implement portfolio optimization techniques under the framework of Modern Portfolio Theory (MPT).

📂 Files

multi_asset_etf_data.xlsx: Source data file with monthly returns of 11 asset classes and a short-term Treasury-bill fund (SHV).
mean_variance_optimization.ipynb: Jupyter Notebook containing all analysis, visualizations, and model implementation.
writeup.pdf: Summary document discussing methodology, findings, and interpretations.
README.md: This file.
🧠 Objective

The objective is to:

Analyze excess returns across asset classes.
Calculate portfolio statistics and compare performance.
Construct and evaluate different allocation strategies (e.g., tangency portfolio, equally-weighted, risk-parity, regularized).
Explore how TIPS (Treasury Inflation-Protected Securities) impact the efficient frontier.
Understand portfolio behavior with and without a risk-free asset.
🛠 Methods

We work primarily with excess returns (asset returns minus SHV), using the excess returns tab in the Excel file. We apply the following steps:

1. Summary Statistics
Calculate and annualize:
Mean excess returns
Volatility (standard deviation)
Sharpe ratios
Identify assets with the best and worst Sharpe ratios.
2. Descriptive Analysis
Correlation matrix of excess returns.
Performance comparison of TIPS vs. domestic and foreign bonds.
3. Tangency Portfolio (Mean-Variance Frontier)
Compute tangency portfolio weights.
Evaluate performance (mean, volatility, Sharpe ratio).
Assess changes in portfolio with and without TIPS.
4. Allocation Strategies
For a target mean excess return of 0.01 (monthly), we construct:

Equally-weighted (EW): Rescaled to match target return.
Risk-parity (RP): Based on inverse variances.
Regularized (REG): Uses shrinkage on covariance matrix.
Tangency Portfolio (MV): From earlier step.
Each strategy's performance is assessed on:

Mean excess return (annualized)
Volatility (annualized)
Sharpe ratio (annualized)
5. Out-of-Sample Performance (Optional, Ungraded)
One-step and rolling out-of-sample tests to evaluate robustness.
Performance tracked for 2016–2024 using rolling estimation windows.
6. No Risk-Free Asset Case (Optional, Ungraded)
Repeat optimization without SHV.
Construct minimum-variance and target return portfolios in a risk-only framework.
