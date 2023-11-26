# Stop Out Monitor

This code is a custom indicator for monitoring the stop out level in a Forex trading account. It calculates the stop out level in both percentage and pips, and checks if the account will stop out for each currency pair.

## How it Works

The indicator uses the following global variables:

- `stopoutLevel`: The stop out level in percentage (default: 50%)
- `stopoutPips`: The stop out level in pips
- `riskTolerance`: The risk tolerance level in percentage (default: 2%)
- `currencyPair`: The current currency pair
- `accountBalance`: The account balance
- `accountRisk`: The account risk level

In the `OnInit` function, the initial values for the global variables are set. The account balance is obtained using the `AccountInfoDouble` function, and the account risk level is calculated based on the risk tolerance level.

The indicator properties are then defined using the `IndicatorSetString`, `IndicatorSetInteger`, and `IndicatorSetDouble` functions.

In the `OnCalculate` function, the stop out level in pips is calculated by multiplying the stop out level with the point value for the current currency pair. 

The account risk level is checked to determine if the account will stop out for each currency pair. If the account risk level is greater than 0, the account risk level and the number of pips required for the currency pair to stop out are printed. If the account risk level is zero, it is indicated that the account risk level is zero.

## Product Description

Stop Out Monitor is a custom indicator designed to help Forex traders monitor their account's stop out level. It calculates the stop out level in both percentage and pips, and provides information on whether the account will stop out for each currency pair.

Key Features:

- Calculates stop out level in both percentage and pips
- Monitors account risk level for each currency pair
- Provides real-time information on account's stop out status

Please note that ForexRobotEasy is not the official developer of this product. This code is provided as a sample that can work as described in the product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [https://forexroboteasy.com/forex-robot-review/stop-out-monitor-review-and-download-the-forex-software-for-real-results/](https://forexroboteasy.com/forex-robot-review/stop-out-monitor-review-and-download-the-forex-software-for-real-results/).
