# Cybertrade Keltner Channels

## Description
This program is designed to implement the Cybertrade Keltner Channels strategy. It calculates the Keltner Channels and checks for trading opportunities based on price crossing above or below the upper and lower bands. It then opens trades accordingly with specified lot size, stop loss, and take profit levels. The program also includes a function to close all open trades.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/cybertrade-keltner-channels-unbiased-review-real-results/). Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Dependencies
This program requires the following libraries:
- Trade.mqh
- Indicator.mqh
- ArrayObj.mqh

## Constants
- SYMBOL: Symbol to trade (e.g., 'EURUSD')
- LOTS: Lot size for trading (e.g., 0.01)
- STOPLOSS: Stop loss level in points (e.g., 100)
- TAKEPROFIT: Take profit level in points (e.g., 200)

## Global Variables
- trade: Trade object
- channels: Array object to store Keltner Channels data

## Functions
- Init: Initializes the trading parameters, such as expert magic number and deviation.
- CalculateChannels: Calculates the Keltner Channels using the iKeltnerChannels function from the Indicator library. Stores the upper band, middle band, and lower band in the channels array.
- CheckOpportunities: Checks for trading opportunities by comparing the current price with the upper and lower bands. Opens a buy trade if the price crosses above the upper band and a sell trade if the price crosses below the lower band.
- CloseTrades: Closes all open trades by iterating over each position and calling the PositionClose function.

## Entry Point
The program's entry point is the OnStart function, which calls the Init, CalculateChannels, CheckOpportunities, and CloseTrades functions in sequence.

Please note that this code is provided as a sample and may require modifications to work in your specific trading environment.
