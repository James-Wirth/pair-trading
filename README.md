# pair-trading

A toy pair trading strategy based on finding a pair of cointegrated stocks, i.e. with stationary spread. A long-short trade is opened when the spread exceeds a certain threshold (in units of standard deviation from zero) and closed when the spread returns to zero or when a stop-loss is triggered.

We use a 10-day rolling average for the spread. The trading threshold is set to $1.2 \sigma$ and the stop-loss threshold is set to $2.5 \sigma$. This toy strategy is shown to be profitable, e.g. with a $z$-score profit of 16.29 for the spread META - $\beta$ MSFT, which were found to be cointegrated with a $p$-value of $\sim 0.0049$.

![zscore](https://github.com/James-Wirth/pair-trading/assets/21970944/985cd9b6-1a0d-4c64-b7cd-cea5c6722c7c)
