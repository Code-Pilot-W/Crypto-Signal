# CryptoSignal - #1 Quant Trading & Technical Analysis Bot

CryptoSignal is a command-line tool that automates cryptocurrency Technical Analysis (TA). It is developed and maintained by a community of traders, engineers, data scientists, and individuals committed to democratizing open access to cryptocurrency trading tools.

## Track over 500 Coins Across Multiple Exchanges
Supports exchanges like Bittrex, Binance, Bitfinex, Coinbase, Gemini, and more, depending on your local financial regulations. Always act responsibly and bear the associated risks.

## Technical Analysis Automated:
- Momentum
- Relative Strength Index (RSI)
- Ichimoku Cloud (Leading Span A, Leading Span B, Conversion Line, Base Line)
- Simple Moving Average
- Exponential Moving Average
- MACD
- MFI
- OBV
- VWAP

## Alerts:
- SMS via Twilio
- Email
- Slack
- Telegram

## Features:
- Modular code for easy trading strategy implementation
- Easy installation with Docker

This tool allows you to implement algorithmic trading and integrate machine learning models for predictive analysis.

## Installing and Running

The following commands are designed to be run in a terminal.

1. Install [Docker CE](https://docs.docker.com/install/).
2. Create a `config.yml` file in your current directory. For customization options, see the section on configuring `config.yml`.
3. Run the application:
   ```bash
   docker run --rm -v $PWD/config.yml:/app/config.yml shadowreaver/crypto-signal:master
   ```
4. Update the application:
   ```bash
   docker pull shadowreaver/crypto-signal:master
   ```

### Configuring `config.yml`

For all configuration options and examples, refer to [docs/config.md](docs/config.md).

## FAQ

### Why does Tradingview show different information than CryptoSignal?
Several factors can cause discrepancies between Tradingview and CryptoSignal:
- Tradingview may have more historical data, which can impact certain indicators.
- Tradingview uses a rolling 15-minute timeframe, which may result in more recent data than CryptoSignal.
- Data collection methods or timeframes might differ between the two platforms, though this is less likely.

### Is CryptoSignal's information accurate?
CryptoSignal relies on [TA-Lib](https://ta-lib.org/index.html), a well-established open-source technical analysis library used in various projects over the past two decades.

## Liability

This tool is intended for educational purposes only. It is not a financial advisor, and none of the contributors to the project are liable for any financial losses. Always do your own research and use simulated trading before applying any strategy with real funds.