# 🛡️ Robo-Advising Portfolio Project

# Low-Volatility Portfolio Construction Engine

Designed to engineer a "Risk-Free" equity portfolio. This tool utilizes Python and Yahoo Finance data to algorithmically select stocks that minimize volatility, beta exposure, and absolute returns, effectively simulating a capital preservation strategy.

## Core Strategy: The "Risk-Free" Approach
Unlike traditional robo-advisors that maximize Sharpe Ratio or Alpha to beat the market, this engine solves for **stability**. The objective is to construct a diversified portfolio of 25 North American equities where the net daily return is as close to 0% as possible, minimizing exposure to market movements.

## Technical Implementation

* **Dynamic Thresholding:** The algorithm adds stocks one by one, calculating the average correlation between the candidate and the existing portfolio.
* **Adaptive Filtering:** It runs simulations across multiple correlation strictness levels to find the perfect balance between diversification and stability.

After generating portfolios across various correlation thresholds, the script selects the portfolio with the **lowest expected daily return**.

---

**Tech Stack:** Python, Pandas, NumPy, yfinance, Matplotlib.
