# 📈 Mean Reversion Trading Strategy - Microsoft (MSFT)

This project implements a simple **Mean Reversion Trading Strategy** using historical price data for **Microsoft (MSFT)**.

---

## 🚀 How it Works

1. **Data Loading:**
   - Upload and read `MSFT.csv`.
   - Set the `Date` as index and clean the data.

2. **Feature Engineering:**
   - Calculate 21-day Simple Moving Average (SMA).
   - Calculate Simple Returns and Log Returns.
   - Create a **Ratios** column (Close price divided by SMA).

3. **Strategy Logic:**
   - Compute important percentiles (15th, 50th, 85th) of Ratios.
   - **Buy Signal** when ratio < 15th percentile.
   - **Sell Signal** when ratio > 85th percentile.

4. **Performance Evaluation:**
   - Compare Cumulative Returns of Buy & Hold vs Mean Reversion.

---

## 🛠️ Libraries Used
- **pandas**: data handling
- **numpy**: numerical computations
- **matplotlib**: plotting and visualization

---

## 📂 Files
- `MSFT.csv`: Historical MSFT data.
- Python script: Your trading logic.

---

## 💡 Future Improvements
- Add transaction costs modeling.
- Optimize thresholds dynamically.
- Test on multiple stocks or asset classes.
