# Optimiser Settings

### 1. Configure Parameters to Test

The optimiser provides six inputs to control the parameter combinations tested.

<img width="501" height="150" alt="Screenshot 2026-10-26 112024" src="https://github.com/user-attachments/assets/c7978399-a7ae-44fc-bfba-a01ff2762bde" />

| Input | Description |
|---|---|
| Start Length | The first Supertrend length to test. |
| Length Iteration | The number of different length values to test. |
| Length Steps | The increment between consecutive length values. |
| Start Multiplier | The first Supertrend multiplier to test. |
| Multiplier Iteration | The number of different multiplier values to test. |
| Multiplier Steps | The increment between consecutive multiplier values. |

**Example configuration:**

```text
Start Length        = 1
Length Iteration    = 5
Length Steps        = 1

Start Multiplier     = 0.5
Multiplier Iteration = 4
Multiplier Steps     = 0.5
```

The optimiser generates the following parameter combinations:

| Length | Multipliers |
|---:|---|
| 1 | 0.5, 1.0, 1.5, 2.0 |
| 2 | 0.5, 1.0, 1.5, 2.0 |
| 3 | 0.5, 1.0, 1.5, 2.0 |
| 4 | 0.5, 1.0, 1.5, 2.0 |
| 5 | 0.5, 1.0, 1.5, 2.0 |

The total number of parameter combinations is calculated as follows:

**Total Combinations = Length Iteration × Multiplier Iteration**

In this example:

`5 × 4 = 20 combinations`

The optimiser tests all 20 combinations and displays the top five results according to the selected sorting criteria and filters.

The default configuration tests **20 lengths × 80 multipliers**, resulting in **1,600 parameter combinations**.

### 2. Sort and Filter Results

#### Sort Basis

<img width="318" height="173" alt="Screenshot 2026-10-26 113329" src="https://github.com/user-attachments/assets/a3c75fde-ccab-4f18-a0a5-09a74b4881b8" />


Choose the performance metric used to rank parameter combinations, such as:

- **Profit and Loss (PnL)**
- **Accuracy**

#### Result Filters

<img width="292" height="302" alt="Screenshot 2026-10-26 113120" src="https://github.com/user-attachments/assets/1f7173e2-d1fa-43c2-a05d-fbaf72a7fd6f" />


Use the following filters to exclude parameter combinations that do not meet your requirements:

- **Minimum Trades**
- **Maximum Trades**
- **Minimum PnL**
- **Minimum Accuracy**

These filters help narrow the results to parameter combinations that satisfy your selected conditions.

### 3. Commission

<img width="289" height="50" alt="Screenshot 2026-10-26 113438" src="https://github.com/user-attachments/assets/e9ce2033-6d0b-4b6e-85f0-a220e281391b" />


The optimiser allows you to include trading commissions in backtest calculations.

Commission is specified as a percentage and applied to both entry and exit transaction values.

**Formula:**

```text
Commission = (Commission Rate / 100)
             × (Entry Price + Exit Price)
```

For example, with a commission rate of 0.1%, an entry price of 100, and an exit price of 110:

```text
Commission = (0.1 / 100) × (100 + 110)
           = 0.21
```

This calculation assumes a quantity of one unit. For larger positions, the calculation must also account for the traded quantity.

## Performance Reports

I will share backtest reports showing how the optimiser's top-ranked parameter combinations perform across different markets and timeframes.

**Performance Reports:** [Insert link]

## Disclaimer

The optimiser ranks parameter combinations based on historical backtest results. **Past performance does not guarantee future results.** Market conditions can change, and parameters that performed well historically may not perform as expected in live markets.

Backtest results may differ from actual trading outcomes due to slippage, commissions, liquidity, and execution conditions.

The Supertrend Optimiser and Supertrend Strategy do not guarantee profitability. Always conduct your own research and testing before making trading decisions. Use both scripts responsibly and at your own risk.
