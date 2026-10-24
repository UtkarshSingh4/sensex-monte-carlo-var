> DRAFT - requires reviewer approval. Prepared by: deterministic template. Number check: all 30 figures traced to model output.

**Subject:** Independent review of the Sensex VaR model (05-Jan-2016 to 23-Oct-2026)

**Scope.** We re-performed and extended the market-risk model using 2660 daily observations from Yahoo Finance via yfinance (^BSESN). 11 data quality controls were run: 0 failed and 4 needed review.

**Key findings**
- Volatility was annualised incorrectly: 14.9% was reported against a correct 18.4%.
- Returns are fat-tailed (excess kurtosis 18.9). The normal model's 1-day 99% VaR of INR 233,833 compares with INR 261,562 under historical simulation, and the historical Expected Shortfall is INR 435,756.
- In a 2409-day out-of-sample backtest, the normal model had 46 exceptions against 24.1 expected and spent 10.0% of days in the Basel Red zone (verdict: Reject).
- The worst day was -13.15% on 23-Mar-2020; the maximum drawdown was -38.1%.

**Overall rating:** 3 High, 4 Medium and 3 Low findings.

**Management actions**
- Adopt Filtered HS as the primary VaR model (31 exceptions; verdict: Accept) and report Expected Shortfall alongside VaR.
- Run the automated data quality controls and backtest every month, with results in the Power BI dashboard.
- For multi-asset clients, report risk contribution as well as weight: equities are 55% of capital but 86% of risk.
