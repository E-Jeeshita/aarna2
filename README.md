# BTC Backtest Strategy - Instructions and Optimizations

## Instructions to Run

1. **Prepare Data:**  
   Ensure the BTC 1-minute OHLCV CSV file is available and correctly placed. Example path:
   ```
   BTC-USDT_1MIN (1).csv
   ```

2. **Install Required Libraries:**  
   If not already installed, use the following commands:
   ```bash
   pip install pandas matplotlib numpy
   ```

3. **Execute the Script:**  
   - Run the Python backtest script provided.
   - The script will print Total PnL, Max Drawdown, and Win Rate.
   - It will also generate and show:
     - The equity curve plot.
     - Price chart with Buy/Sell signals.

4. **Output Files:**  
   - Trade logs are saved automatically as `trade_logs.csv` in the same directory.

---

## Optional Optimizations

### 1. **Transaction Fees & Slippage**
- Add a realistic fee by subtracting a percentage (like 0.1%) from every trade.
- Adjust the capital and position size calculations accordingly.

### 2. **Stop Loss / Take Profit**
- Implement logic to exit trades early based on predefined thresholds.

### 3. **Dynamic Position Sizing**
- Instead of using 100% capital for each trade, vary trade sizes based on volatility or signal strength.

### 4. **Strategy Improvements**
- Add more indicators (e.g., RSI, MACD) to reduce false signals.
- Use different timeframes or combine multiple timeframes for more robust signals.

### 5. **Performance Reporting**
- Add metrics like Sharpe ratio, Sortino ratio, and profit factor for deeper analysis.



