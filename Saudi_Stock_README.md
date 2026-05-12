# Saudi Stock Market (Tadawul) — CAPM & Risk-Return Analysis
### Financial Analysis using Python | CAPM · Sharpe Ratio · Beta · Alpha

---

## Project Overview

This project analyzes **13 Tadawul-listed stocks** across key Saudi sectors — energy, banking, telecom, and Vision 2030 companies — using Python and the Capital Asset Pricing Model (CAPM) to rank stocks by risk-adjusted return.

**Author:** Talah Almualad  
**Tools:** Python · yfinance · pandas · numpy · matplotlib · scipy

---

## Key Questions Answered

- Which Saudi stocks deliver the best **risk-adjusted return** (Sharpe Ratio)?
- How sensitive is each stock to **market movements** (Beta)?
- Which stocks generate **alpha** above the market's expected return?
- What is the **CAPM expected return** for each stock?

---

## Stocks Analyzed

| Sector | Companies |
|--------|-----------|
| **Energy & Petrochemicals** | Saudi Aramco · SABIC · Petro Rabigh |
| **Banking** | Al Rajhi Bank · SAMBA · Al Jazira Bank |
| **Vision 2030** | ACWA Power · Elm Company · Saudi Tadawul Group |
| **Consumer & Retail** | Savola Group · Jarir Bookstore |
| **Telecom** | STC · Mobily |

---

## Methodology

### 1. Data Collection
- Historical price data fetched via **yfinance** (2021–2024)
- Benchmark: **Tadawul All Share Index (^TASI)**
- Risk-Free Rate: **5%** (Saudi repo rate)

### 2. Return & Risk Metrics
- Annualized return and volatility for each stock
- Log returns for accurate compounding

### 3. CAPM Analysis
- **Beta** — market sensitivity via linear regression
- **Alpha** — excess return above CAPM expectation
- **CAPM Expected Return:** `E(R) = Rf + β(Rm - Rf)`

### 4. Risk-Adjusted Performance
- **Sharpe Ratio:** `(Return - Rf) / Volatility`
- Stocks ranked from highest to lowest Sharpe Ratio

---

## Visualizations

The project produces 5 charts:

- **Sharpe Ratio Ranking** — horizontal bar chart ranking all stocks
- **Risk vs Return Scatter** — color-coded by Sharpe Ratio
- **Beta Analysis** — market sensitivity per stock
- **Actual vs CAPM Expected Return** — comparison per stock
- **Top 5 Summary Table** — best risk-adjusted performers

---

## Tech Stack

```
Python 3.x
├── yfinance      — Tadawul stock data extraction
├── pandas        — data manipulation
├── numpy         — numerical computations
├── matplotlib    — data visualization
├── seaborn       — enhanced charts
└── scipy         — linear regression (Beta calculation)
```

---

## How to Run

### Option 1: Google Colab (Recommended)
1. Open [Google Colab](https://colab.research.google.com)
2. Upload `Saudi_Stock_Market_Analysis.py`
3. Run all cells

### Option 2: Local
```bash
pip install yfinance pandas numpy matplotlib seaborn scipy
python Saudi_Stock_Market_Analysis.py
```

---

## Key Findings

- Analysis covers **13 Saudi stocks** across **5 sectors** (2021–2024)
- CAPM Beta identifies which stocks amplify or dampen market movements
- Stocks with **Alpha > 0** generate returns above what CAPM predicts
- Sharpe Ratio ranking provides actionable insight for portfolio construction

---

## Related Project

- [Alternative Investment Portfolio Optimization](https://github.com/Talah2/alternative-investment-portfolio) — CAPM · Efficient Frontier · Monte Carlo

---

## Author

**Talah Almualad**  
Finance Graduate | King Abdulaziz University | GPA: 4.74/5  
CO-OP: Petro Rabigh (Saudi Aramco & Sumitomo Chemical JV)  
[LinkedIn](https://linkedin.com/in/talah-almualad-2b3902329) · [GitHub](https://github.com/Talah2)
