# ADR Alert Dashboard MT5

This code is a custom indicator for MetaTrader 5 (MT5) platform that calculates the Average Daily Range (ADR) and generates alerts when the price exceeds a custom upper level above the ADR. 

## Input Parameters
- ADR_Period: The period for calculating the ADR (default value: 14).
- ADR_Multiplier: The multiplier for custom levels above the ADR (default value: 1.5).

## Initialization
The indicator initializes by calculating the ADR using the iATR function, which calculates the Average True Range (ATR) indicator. The ADR is calculated for the specified period (ADR_Period) and for the D1 (daily) timeframe. The custom upper level for alerts is also calculated by multiplying the ADR by the ADR_Multiplier.

## Indicator Iteration
The indicator iterates through the price data and checks if the current high price exceeds the custom upper level. If it does, an alert is generated with the message 'Price exceeds ADR: [high price]'. The high price is converted to a string using the DoubleToString function and the number of decimal digits (_Digits) is used for formatting.

## Deinitialization
The deinitialization function is empty in this code but can be used to perform any necessary cleanup tasks.

Please note that Forex Robot Easy is not the official developer of this product. We only provide sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - ADR Alert Dashboard MT5](https://forexroboteasy.com/forex-robot-review/review-adr-alert-dashboard-mt5-real-results-and-download-available/).
