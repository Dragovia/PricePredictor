This is a sophisticated non-AI algorithmic trading system that predicts cryptocurrency price movements for the HYPE perpetual futures contract on Hyperliquid exchange.


Core Purpose
Predicts whether the price will move up or down across multiple time horizons (10s, 30s, 60s) using mathematical models, then logs predictions and performance to CSV.

Data Collection (WebSocket Connection)

Connects to Hyperliquid's WebSocket API
Subscribes to two data streams:

Order book updates (L2 book): bid/ask prices and sizes
Trade feed: executed trades with price, size, and side (buy/sell)


Converts various timestamp formats to Unix seconds
