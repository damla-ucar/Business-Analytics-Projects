# crypto-arbitrage-cointegration
Market-neutral cryptocurrency portfolio &amp; trading strategy using cointegration and dynamic mean-reversion.

# 📈 Market-Neutral Cryptocurrency Portfolio & Trading Strategy

> **Project for Business Analytics (Spring 2024-2025)**  
> Using statistical arbitrage and cointegration to design a market-neutral trading strategy on hourly crypto data.

---

## 🧰 Technologies & Methods
- Python (Pandas, statsmodels, scikit-learn)
- Time series analysis & cointegration
- Engle–Granger two-step method
- Statistical arbitrage & mean-reversion
- Backtesting & rolling window dynamic strategy

---

## 📊 Project Overview

This project constructs a **cointegrated, market-neutral cryptocurrency portfolio** using the Engle–Granger two-step method, following:

> Leung, T. and Nguyen, H. (2019). *Constructing cointegrated cryptocurrency portfolios for statistical arbitrage.*

Then:
- Designs a trading strategy based on mean-reversion of the spread.
- Evaluates its performance over historical train/test data.
- Develops an **improved dynamic trading strategy** using rolling window statistics.

---

## 📂 Data

- Hourly historical prices from Binance API.
- Period: **Jan 1, 2023 – Jan 1, 2025**
- Train set: up to Sep 1, 2024 (~84%)
- Test set: Sep 1, 2024 onward (~16%)

---

## ⚙️ Methodology

### 1️⃣ Data Preparation & Stationarity Tests
- Collected hourly data for BNBUSDT, SOLUSDT, ALPHAUSDT, ALPINEUSDT, DOGEUSDT, etc.
- Performed ADF, PP, KPSS tests:
  - Non-stationary in levels
  - Stationary in first differences


---

### 2️⃣ Engle–Granger Cointegration
- Used `BNBUSDT` as dependent; others as independents.
- OLS regression → R² ≈ 0.882; predictors significant.
- Residuals tested → stationary → confirmed cointegration.

---

### 3️⃣ Trading Strategy

Constructed spread:

Spread_t = BNBUSDT_t - b1·ALPHAUSDT_t - b2·ALPINEUSDT_t - b3·DOGEUSDT_t


- Mean-reversion trading rule:
  - Go long when spread < μ − c·σ
  - Go short when spread > μ + c·σ
- Tried thresholds c ∈ [0.5, 0.75, 1.0, 1.25, 1.5]
- Threshold=1.0 chosen as best balance.

---

### 4️⃣ Backtesting & Results

**Test set results:**
- Total Trades: 3
- Net P&L: \$226.56
- Avg Trade P&L: \$75.52

---

## ⭐ Bonus: Dynamic Strategy

To adapt to shocks:
- Used rolling window to update mean & std.
- Dynamic z-score → more responsive trading.
- Better adapts to spread divergence.

---

## ✅ Conclusion

- Successfully built a cointegrated, market-neutral crypto portfolio.
- Designed & backtested a mean-reversion strategy.
- Explored a dynamic variant to adapt to market shifts.

