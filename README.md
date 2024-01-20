# Waddah Attar Explosion MT4 - ReadMe

## Description
This code is a custom indicator and trading robot for the MetaTrader 4 (MT4) platform. It is based on the Waddah Attar Explosion formula and is developed by the Forex Robot Easy Team. The indicator calculates trend power and explosion power, and the trading robot uses these values to generate buy and sell signals.

## Indicator Functions
1. **CalculateTrendPower(bar):** This function calculates the trend power based on the Waddah Attar Explosion formula. It takes the bar index as a parameter and stores the trend power value in the `trendPowerBuffer` array.

2. **CalculateExplosionPower(bar):** This function calculates the explosion power based on the Waddah Attar Explosion formula. It takes the bar index as a parameter and stores the explosion power value in the `explosionPowerBuffer` array.

## Trading Robot Functions
1. **IsBuySignal(bar):** This function checks if there is a buy signal based on the explosion power value. If the explosion power value is higher than the buy threshold, it returns true; otherwise, it returns false.

2. **IsSellSignal(bar):** This function checks if there is a sell signal based on the explosion power value. If the explosion power value is lower than the sell threshold, it returns true; otherwise, it returns false.

3. **IsExitBuySignal(bar):** This function checks if there is an exit buy signal. If the explosion power value is negative, it returns true; otherwise, it returns false.

4. **IsExitSellSignal(bar):** This function checks if there is an exit sell signal. If the explosion power value is positive, it returns true; otherwise, it returns false.

## OnTick Function
The `OnTick` function is the main function that is called on each tick of the market. It calculates the trend power and explosion power for the current bar using the `CalculateTrendPower` and `CalculateExplosionPower` functions. It then checks for buy, sell, exit buy, and exit sell signals using the corresponding functions. If a signal is detected, the appropriate trade setup can be executed.

## Product Description
This code is a sample implementation of the Waddah Attar Explosion MT4 indicator and trading robot. It is developed by the Forex Robot Easy Team, but ForexRobotEasy is not the official developer of this product. This code showcases how the indicator and trading robot can be implemented and used.

For detailed reviews and trading results of the official product, please visit the following link: [Waddah Attar Explosion MT4 - Forex Trading Power Tool Review](https://forexroboteasy.com/forex-robot-review/waddah-attar-explosion-mt4-forex-trading-power-tool-review/).

Note: To find the official developer of this product, please refer to MQL5.
