# Gold Trading Artist

Gold Trading Artist is a Forex trading robot developed by the Forex Robot Easy Team. It is designed to trade the gold market using a high probability strategy based on a moving average indicator.

## Input Parameters

The following input parameters can be customized:

- **SpreadLimit**: The maximum allowable spread for trading.
- **MM**: Enable or disable money management.
- **AutoLotSize**: The percentage of the account balance to be used for position sizing if money management is enabled.
- **ManualLotSize**: The fixed lot size to be used for position sizing if money management is disabled.
- **StopLoss**: The stop loss level for each trade.
- **MAPeriod**: The period of the moving average indicator.
- **MATimeframe**: The timeframe of the moving average indicator.
- **MAMethod**: The method used to calculate the moving average.

## Global Variables

The following global variables are used:

- **ticket**: The trade ticket number.
- **lotSize**: The calculated lot size for each trade.

## Custom Indicator Initialization

The `OnInit()` function is responsible for initializing the indicator. It performs various checks on the input parameters to ensure they are within valid ranges. If any of the input parameters are invalid, the indicator initialization fails.

## Custom Indicator Iteration

The `OnTick()` function is called on each tick of the market. It calculates the moving average value, the current bid and ask prices, and the current spread. It then checks whether the current spread exceeds the specified limit. If the spread is within the limit, it calculates the lot size based on the chosen money management option. If money management is enabled, the lot size is calculated as a percentage of the account balance. If money management is disabled, the lot size is set to the manually specified value.

If there is an open position, the function checks if the position is profitable. If it is, a trailing stop is set to protect the profits. If there is no open position, the function checks the current bid price against the moving average. If the bid price is above the moving average, a buy order is placed. If the bid price is below the moving average, a sell order is placed.

## Product Description

Gold Trading Artist is a Forex trading robot developed by the Forex Robot Easy Team. It utilizes a high probability strategy based on a moving average indicator to trade the gold market. The robot is designed to be used on the MetaTrader 4 platform.

The robot offers several customizable input parameters, including the maximum allowable spread, money management options, stop loss level, and moving average parameters. Traders can choose to enable or disable money management and specify the lot size calculation method. The robot also allows traders to set their preferred stop loss level and adjust the period and method of the moving average indicator.

Gold Trading Artist is a reliable and efficient trading robot that aims to generate consistent profits in the gold market. It is suitable for both beginner and experienced traders who are looking for an automated solution to trade gold.

Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please refer to the MQL5 community or the website mentioned in the header.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-gold-trading-artist-a-winning-forex-software-with-high-probability-strategy/).
