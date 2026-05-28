# SigmaFlow — Signal-to-Execution Agent

Signal-to-Execution Agent built on SoSoValue API + SoDEX, powered by Claude AI.
SoSoValue Buildathon 2026 — Wave 1 Submission

Live Demo: https://younjungg066.github.io/sigmaflow-agent/

---

## What is SigmaFlow?

SigmaFlow is an agentic finance application that bridges the gap between market intelligence and on-chain execution. It takes raw market data from SoSoValue API, runs AI-powered signal analysis via Claude, and routes trade orders directly through SoDEX — all in one unified interface.

The goal: a single-person team can operate like a fund manager.

---

## How It Works

1. Fetch real-time price and indicator data via SoSoValue API
2. Load SSI Index data (Top10, DeFi) from SSI Protocol
3. Compute signal composite scores — momentum, mean-reversion, sentiment
4. Send all context to Claude for natural-language market analysis
5. Display verdict (BUY / SELL / HOLD) with confidence score
6. User confirms — order submitted to SoDEX on-chain orderbook

---

## Features

- Live market dashboard with real-time prices for BTC, ETH, SOL, SSI indexes
- Three signal types: momentum, mean reversion, sentiment scoring
- Technical indicators: RSI, MACD, Bollinger Bands, Volume ratio
- AI analysis engine: Claude generates market context and trading verdict
- Order execution wired to SoDEX API (testnet supported)
- Agent flow log tracking every step in real time
- Portfolio tracker showing total value, available USDC, open positions

---

## APIs Used

| API | Purpose |
|-----|---------|
| SoSoValue API | Market data, news, SSI index prices |
| SSI Protocol | On-chain index exposure (Top10, DeFi) |
| SoDEX API | On-chain orderbook execution via ValueChain L1 |
| Anthropic Claude | AI signal analysis and trade recommendation |

---

## Setup

Open index.html directly in a browser — works in demo mode without any API keys.

To connect live APIs, click Configure in the top-right corner and enter:
- SoSoValue API Key — register at sosovalue.com
- SoDEX API Key — testnet requires no deposit; mainnet requires Buildathon whitelist
- Anthropic API Key — enables live Claude analysis

Keys are stored in browser session only.

---

## Wave Progress

Wave 1 (current)
- Core UI: dashboard, chart, signal cards, order form
- Demo mode with simulated live prices
- AI analysis engine with Claude integration
- SoDEX order submission flow
- Agent flow log

Wave 2 (planned)
- Real SoSoValue API integration with live news and market data
- SoDEX testnet order execution
- Signal backtesting module
- Auto-trigger when confidence exceeds threshold

---

## Team

younjungg066 — Solo builder — levantu170605@gmail.com

---

## License

MIT
