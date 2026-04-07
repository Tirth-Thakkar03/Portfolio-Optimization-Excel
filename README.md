# Portfolio-Optimization-Excel
Markowitz Mean-Variance Portfolio Optimization — 14 stocks, GMV framework, Excel

📊 Markowitz Mean-Variance Portfolio Optimization
Independent Research Project | MS Finance, University of Texas at Dallas
Data: Yahoo Finance | Period: January 2022 – October 2025 | Frequency: Weekly

🔍 Overview
This project implements a Global Minimum Variance (GMV) Portfolio Optimization framework from scratch in Microsoft Excel, applying Harry Markowitz's Modern Portfolio Theory to a universe of 14 U.S. equities split across two distinct risk profiles:
UniverseStocksMega-Cap (7)AAPL, MSFT, NVDA, GOOGL, TSLA, AMZN, METAHigh-Volatility (7)SNAP, CRWD, COIN, UBER, PLTR, ROKU, ZM
Three separate GMV portfolios are constructed and compared:

Portfolio 1 — Mega-Cap only
Portfolio 2 — High-Volatility only
Portfolio 3 — Combined (14 stocks)

💡 Key Findings

Diversification confirmed — The combined 14-stock portfolio achieved lower variance (0.000786) than either sub-portfolio alone, validating cross-universe diversification benefits.
Microsoft dominates mega-cap — MSFT carries ~78% weight in the mega-cap GMV due to its relatively low variance versus peers.
ZM and UBER anchor high-vol — Their lower cross-correlations with other high-volatility stocks make them the most efficient holdings in that universe.
Short positions — NVDA, TSLA, META, CRWD, COIN, and ROKU all receive negative weights, indicating they add more risk than return in this sample period.
High-vol universe underperformed — Negative expected return (-1.3% weekly) and negative Sharpe ratio (-11.99) across 2022–2024 reflects the difficult environment for speculative growth stocks.
Best combined outcome — The 14-stock portfolio delivers the highest Sharpe ratio (14.57) and lowest standard deviation (2.80%), demonstrating that combining both universes meaningfully improves the risk-return tradeoff.


🚧 Work in Progress
Currently extending the model to include full bull and bear case scenario analysis — stress-testing how each portfolio responds to a sudden market surge or a sharp market drawdown. The objective is to evaluate not just optimal weights under normal conditions, but portfolio resilience when market conditions shift dramatically in either direction.

✅ Bull case (positive returns ×1.2, negative returns ×0.8) — complete
🔄 Bear case (positive returns ×0.8, negative returns ×1.2) — in progress
🔄 Efficient frontier visualization — in progress


🛠️ Tools Used

Microsoft Excel — Advanced formulas, MINVERSE, MMULT, array functions
Yahoo Finance — Historical weekly price data
Data Period — January 2022 to October 2025 (~130 weekly observations per stock)


⚠️ Limitations & Notes

Short selling is permitted in this model (no long-only constraint)
Sharpe ratios are calculated on a weekly basis and are not annualized (multiply by √52 for annualized equivalent)
Risk-free rate assumed to be 0; substituting a T-bill rate would lower Sharpe ratios
Model is in-sample only; no out-of-sample backtesting conducted
Estimation error in the covariance matrix is not corrected (e.g., no shrinkage estimator)


👤 Author
Tirth Thakkar
MS Finance Candidate | University of Texas at Dallas
tirth.m.thakkar@gmail.com
