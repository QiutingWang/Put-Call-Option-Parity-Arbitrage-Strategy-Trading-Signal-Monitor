# Put Call Option Parity Arbitrage Strategy Trading Signal Monitor

## Introduction
This project is to monitor the arbitrage opportunity of stocks, options, and futures every second based on Put-Call parity in the Chinese stock market. Here, we focus on ETFs whose indexes are SSE 50, CSI 300, and CIC 500. Whenever it finds a trading signal, it would record it, do the trading operations and make profits. However, there are <u>small profits and small chances</u> to get a trading signal.
## Main
- Every 20 seconds we download all the etf futures, options, and stocks index data, then extract them into a .csv file.
- Data Source: Wind database
- Financial Thorey: $P+S=C+\frac{K}{(1+Rf)^T}+D$
  - if the relationship does not hold, there exists an arbitrage opportunity.

And all the details for calculation, you can see in CalStat.py
## Reference:
- [QuantConnect: PUT-CALL PARITY AND ARBITRAGE STRATEGIES](https://www.quantconnect.com/learning/articles/introduction-to-options/put-call-parity-and-arbitrage-strategies)

