# Financial Risk & Scenario Analysis (Python)

This project implements a Python-based portfolio risk and scenario analysis framework to evaluate
volatility, downside risk, and capital buffer requirements under normal and stressed market conditions.

The objective is to translate market risk into decision-relevant capital insights.

---

## Portfolio Setup
- **SPY (US Equities):** 60%
- **AGG (US Aggregate Bonds):** 30%
- **GLD (Gold):** 10%
- **Data Frequency:** Daily
- **Lookback Period:** ~5 years
- **Confidence Levels:** 95% and 99%

---

## Methodology
- Constructed daily portfolio returns using capital-weighted asset returns
- Computed core risk metrics:
  - Annualized volatility
  - Value at Risk (VaR)
  - Conditional Value at Risk (CVaR)
  - Maximum drawdown
- Designed stress scenarios:
  - Mild equity shock
  - Severe equity shock
  - Volatility spike
- Recomputed risk metrics under each scenario
- Converted tail risk into dollar-based capital buffer estimates

---

## Key Outputs
- Portfolio return distribution (histogram)
- Scenario-based risk comparison table
- Capital buffer requirements under baseline and stress conditions

---

## Key Insight
Stress scenarios—particularly volatility shocks—require approximately **2× higher capital buffers**
than baseline conditions, highlighting uncertainty as the dominant driver of downside risk.

---

## Tools Used
Python, pandas, numpy, yfinance, matplotlib