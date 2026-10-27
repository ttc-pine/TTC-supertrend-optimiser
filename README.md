# Supertrend Optimiser

## What Is the Supertrend Optimiser?

The **Supertrend Optimiser** is a tool designed to help traders find suitable input parameters for the Supertrend indicator. It backtests **1,600 different parameter combinations** and identifies the best-performing parameters based on the selected optimisation criteria.

The performance and behaviour of technical indicators can vary significantly across different symbols and timeframes. As a result, finding suitable Supertrend settings for a particular market and timeframe can be challenging and time-consuming.

The Supertrend Optimiser addresses this problem by comparing the backtest results of 1,600 parameter combinations and identifying the best-performing settings for a specific symbol and timeframe in just seconds.

## How to Use the Supertrend Optimiser

The Supertrend Optimiser identifies the best-performing parameters for the symbol and timeframe on which it is applied, based on your selected optimisation criteria.

### Steps

1. Add the **Supertrend Optimiser** to your chart.
2. Configure the optimisation settings according to your requirements.
3. Run the optimiser and note the best-performing parameters.
4. Enter the selected parameters into the **Supertrend Strategy**.
5. Review the strategy's backtest report to determine whether its performance meets your requirements.
6. If the results are satisfactory, consider using the Supertrend for further analysis or as part of your trading strategy.


### Video demonstration:
https://github.com/user-attachments/assets/647ed400-502b-4367-8cf3-b2564a9ee0e0


### Applications

Beyond using the Supertrend as a trading strategy, you can also use it for technical analysis:

- **Trailing Stop-Loss:** Use the Supertrend line as a reference for managing trailing stop-loss levels.
- **Trend Detection:** Identify potential bullish and bearish market trends.
- **Dynamic Support and Resistance:** Use the Supertrend line as a potential dynamic support or resistance level.

## Supertrend Optimiser Settings

The Supertrend Optimiser provides several settings that allow you to customise the optimisation process.

### 1. Parameter Range

<img width="501" height="150" alt="Screenshot 2026-10-26 112024" src="https://github.com/user-attachments/assets/629bc108-7d8e-4aaf-9c8f-400d19b2daab" />

Configure the range of Supertrend parameters to be tested during optimisation. This allows you to control which parameter combinations are included in the analysis.

### 2. Optimisation Criteria

<img width="318" height="173" alt="Screenshot 2026-10-26 113329" src="https://github.com/user-attachments/assets/c9222d88-546f-4a4d-a994-5ebbd6ddf0a3" />

Choose the performance metric used to identify the best parameters, such as **Profit and Loss (PnL)** or **Accuracy**.

### 3. Result Filters

<img width="292" height="302" alt="Screenshot 2026-10-26 113120" src="https://github.com/user-attachments/assets/1e066efa-fef3-431d-b08c-fe94cf34443e" />

Apply filters to exclude parameter combinations that do not meet your specified criteria. Only the results satisfying the selected filters will be retained.

### 4. Commission Settings

<img width="289" height="50" alt="Screenshot 2026-10-26 113438" src="https://github.com/user-attachments/assets/d6464ea6-3de0-49b6-a8f9-5227e80c04e0" />

Include trading commissions in the backtests to account for transaction costs when evaluating the performance of different parameter combinations.

For a detailed explanation of each setting, refer to the [Supertrend Optimiser Settings Guide](optimiser-settings-guide/optimiser-settings-guide.md).

## Performance Reports

This are the backtest reports of supertrend strategy(for best-performing Supertrend parameters identified by the optimiser) in chart available data for NIFTY50 index across various timeframes(1M, 3M, 5M, 10M, 15M, 30M, 1H, 4H and 1D).
<img width="1260" height="620" alt="B3nTn" src="https://github.com/user-attachments/assets/1f30a808-871f-4c03-b299-09b2895d0caf" />


### ⚠️ Important Note on Backtesting

Due to TradingView's limitations, the optimiser can backtest parameter combinations only on the historical data available(around 20,000 bars/candles) on the chart. Therefore, the top-performing parameters identified by the optimiser are based on the available chart data and may not be the best-performing parameters across the entire historical period.

**For more reliable evaluation, we recommend validating the selected parameters using TradingView's Deep Backtesting feature** before using them in live trading. This helps you assess their performance over a more extensive historical period.

Based on our testing, most of the parameter combinations identified by the optimiser have also performed well across the full chart history when evaluated using Deep Backtesting. However, past performance does not guarantee future results.


## Disclaimer

The Supertrend Optimiser identifies the best-performing parameters based on historical backtest results. However, **past performance does not guarantee future results**. Market conditions can change, and parameters that performed well historically may not perform as expected in live trading.

Backtest results may also differ from actual trading results due to factors such as slippage, transaction costs, and execution conditions.

The Supertrend Optimiser and Supertrend Strategy are analytical tools and do not guarantee profitability. Use both scripts responsibly and at your own risk. Always conduct your own research and testing before making trading decisions.
