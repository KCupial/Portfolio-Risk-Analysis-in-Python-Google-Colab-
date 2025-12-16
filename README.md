## Financial Time Series Analysis – Log Returns and Risk Measures

This project presents an exploratory and statistical analysis of daily stock returns
for selected companies (BHP, Pfizer, LVMH).

The objective of the analysis is to:
- examine the statistical properties of log returns,
- assess distributional assumptions,
- identify outliers and autocorrelation,
- evaluate market risk using VaR and CVaR measures.

The project is designed as a documentation-first analysis, with full results and interpretations
provided in the Python notebook.

---

## Data Source
Market data is downloaded automatically from Yahoo Finance using the `yfinance` library.
The analysis uses daily closing prices.

---

## Selected Results

### Closing price time series
<img width="897" height="374" alt="image" src="https://github.com/user-attachments/assets/dccab9cc-23eb-4a8f-945a-5e4397fb44dd" />


The chart illustrates the evolution of daily closing prices and highlights long-term trends
and periods of increased volatility.

---

### Distribution of logarithmic returns
<img width="896" height="371" alt="image" src="https://github.com/user-attachments/assets/ce003825-8882-4157-a87a-0b47ce3ad912" />


Log returns exhibit heavy tails and deviations from normality, indicating that
parametric risk measures may underestimate tail risk.

---

### Outliers in log returns
<img width="893" height="368" alt="image" src="https://github.com/user-attachments/assets/ff9d8bcc-b713-4e7d-a2d9-d8c1003a52e0" />

Extreme observations are identified using the IQR method, highlighting periods
of unusually high market stress.

---

## Documentation
The full analysis, including methodology, charts, statistical tests, and interpretations,
is available in the notebook:

- `financial_time_series_analysis.ipynb`

---

## Tools & Technologies
- Python (pandas, numpy, matplotlib, scipy, statsmodels)
- Yahoo Finance (`yfinance`)
- Jupyter / Google Colab
