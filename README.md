# News Catcher Pro

This code is for a program called News Catcher Pro developed by the Forex Robot Easy Team. The purpose of this program is to identify intraday seasonal volatility patterns caused by high-impact news events and enter the market based on these patterns. 

## How it Works

The program uses the MQL5 language and is designed to be run on the MetaTrader platform. It consists of several functions that work together to identify news events and volatility patterns and enter the market accordingly.

### identifyVolatilityPatterns() Function

This function takes a datetime parameter representing the time of a high-impact news event. It is responsible for implementing the logic to identify volatility patterns caused by this event. Currently, the function simply returns true, indicating that volatility patterns have been identified.

### enterMarket() Function

This function takes a symbol and a timeframe as parameters. It is responsible for implementing the logic to enter the market based on the identified volatility patterns. The function prints a message indicating the symbol, the timezone, and the timeframe being used.

### OnTick() Function

This is the main function of the program and is called on every tick of the market. It initializes an array of currency pairs and sets an optimal timeframe. It then iterates through each currency pair and performs the following steps:

1. Checks if the symbol is allowed for trading. If not, it prints a message indicating that the symbol is not allowed and continues to the next iteration.

2. Gets the next high-impact news event for the symbol.

3. Checks if there is a high-impact news event. If there is, it checks if the current time is shortly before the event.

4. If the current time is shortly before the event, it calls the identifyVolatilityPatterns() function to identify volatility patterns.

5. If volatility patterns are identified, it calls the enterMarket() function to enter the market.

### OnTick_MT5() Function

This is the MT5 version of the OnTick() function. It simply calls the OnTick() function.

## Product Description

News Catcher Pro is a professional forex trading software developed by the Forex Robot Easy Team. It is designed to help traders identify intraday seasonal volatility patterns caused by high-impact news events and enter the market based on these patterns.

With News Catcher Pro, traders can take advantage of the increased volatility and potential profit opportunities that occur during high-impact news events. The program uses advanced algorithms to analyze market data and identify patterns that have historically resulted in significant market movements.

The program is easy to use and can be run on the MetaTrader platform. It provides real-time notifications of high-impact news events and automatically enters the market based on the identified volatility patterns. Traders can customize the program to suit their trading preferences by selecting the currency pairs and timeframes they want to trade.

Please note that ForexRobotEasy is not the official developer of News Catcher Pro. We are only providing this sample code to demonstrate how the program works. To find the official developer of News Catcher Pro and access detailed reviews and trading results, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-news-catcher-pro-a-professional-forex-traders-analysis-of-this-forex-software/).
