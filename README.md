# Testing Normality in Log Returns of Financial Assets

This project explores the assumption of normality in the log returns of individual stocks and constructed portfolios — a core principle in many mathematical finance models.

---

##  Project Objectives

1. **Test normality** of full-period log returns for 10 individual stocks, data generated using yfinance.
2. **Use rolling windows** to identify periods when returns appear Gaussian.
3. **Trim outliers** (top/bottom 1% and 3%) to improve distribution shape.
4. **Construct a portfolio** from trimmed, normally distributed assets.

---

## Key Results

- None of the full-period log return distributions were normal.
- XOM showed the most frequent local normality (80%+ of rolling windows).
- After 3% trimming, 5 stocks passed the Anderson-Darling test:  
  `JNJ, KO, NVDA, TSLA, XOM`
- A portfolio built from these trimmed returns **passed all normality tests**.

---

## Statistical Methods Used

- **Shapiro-Wilk Test**
- **Jarque-Bera Test**
- **Anderson-Darling Test**
- 126-day **rolling window** analysis

---

## Visualizations

- Histogram + KDE plots
- Q-Q plots
- Boxplots
- Rolling pass-rate bar chart

---

## Tools & Libraries

- Python 🐍
- `pandas`, `numpy`, `matplotlib`, `seaborn`  
- `scipy.stats`, `statsmodels.api`
- `yfinance` for stock data

---
## Report 
- see the "report.pdf" for the project report 
- "code.ipynb" is the jupyter notebook for this project
