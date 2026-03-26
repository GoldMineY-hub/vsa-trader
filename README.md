# VSA Trader

> 🇳🇱 **Deze tool is volledig in het Nederlands — gebouwd voor day traders in Nederland, België en heel Europa.**

A free **Volume Spread Analysis (VSA)** tool for Dutch and Belgian stock traders. Analyse US and AEX stocks in real-time using professional VSA signals, VWAP, EMA, ATR and CVD — directly from your browser, no account required.

🌐 **Live app:** [goldminey-hub.github.io/vsa-trader](https://goldminey-hub.github.io/vsa-trader/)

---

## What does it do?

Type any stock ticker — `AAPL`, `TSLA`, `NVDA` or `ASML.AS` — and get a full VSA report within seconds:

- 20+ VSA signal types automatically detected
- VWAP, EMA-20, EMA-50, ATR and CVD analysis
- Candlestick chart with signal overlays
- Trend strength and bias (bullish / bearish / neutral)
- Stop-loss suggestion based on ATR

---

## Features

| Feature | Description |
|---|---|
| 📊 **VSA Signal Detection** | Stopping Volume, No Supply, No Demand, Demand Surge, Shake Out, Up-Thrust and more |
| 📍 **VWAP** | Volume-weighted average price — above = bullish, below = bearish |
| 📈 **EMA-20 / EMA-50** | Trend direction and momentum |
| 📐 **ATR** | Average True Range for stop-loss calculation |
| 🌊 **CVD** | Cumulative Volume Delta — buying vs selling pressure |
| 🔔 **Volume Alert Scanner** | Automatically scans 40+ stocks for volume spikes and price moves |
| 📌 **Watchlist** | Track up to 20 stocks with live price, bias tag and sparkline |
| 📓 **Trade Journal** | Log trades with entry, exit, stop-loss, win rate and personal stats |
| 📚 **Learning Library** | Full Dutch explanations of VSA, VWAP, EMA, ATR, candlesticks and trading psychology |
| 🧠 **Interactive Quiz** | Test your VSA knowledge |

---

## VSA Signals Explained

| Signal | Meaning |
|---|---|
| **Stopping Volume** | High volume, small spread at support — institutions absorbing sell pressure |
| **No Supply** | Low volume down bar — sellers exhausted, potential reversal up |
| **No Demand** | Low volume up bar — buyers weak, potential reversal down |
| **Demand Surge** | High volume, wide spread closing near high — strong buying |
| **Shake Out** | Price pushed below support, closes back up — bullish trap |
| **Up-Thrust / Rejection** | Price pushed above resistance, closes back down — bearish trap |
| **Climactic Action** | Extreme volume spike — possible trend exhaustion |
| **Bullish Absorption** | High volume at support with little price reaction — hidden strength |

---

## Who is this for?

- 🇳🇱 Dutch and Belgian day traders and swing traders
- Beginners learning VSA concepts step by step
- Intermediate traders looking to confirm entries and exits
- Anyone trading US stocks (NYSE, NASDAQ) or AEX stocks from Europe

---

## Supported Markets

| Market | Example tickers |
|---|---|
| **NYSE / NASDAQ** | AAPL, TSLA, NVDA, AMD, PLTR, SOFI, MARA, NIO |
| **AEX (Amsterdam)** | ASML.AS, PHIA.AS, HEIA.AS, ADYEN.AS |
| **ETFs** | SPY, QQQ, IWM |

---

## Getting Started

### Option A — Use it directly (no setup)
Open the live app at [goldminey-hub.github.io/vsa-trader](https://goldminey-hub.github.io/vsa-trader/). Analysis takes 20–30 seconds via the public server.

### Option B — Set up your own Cloudflare Worker (recommended)
Get analysis results in **1–2 seconds** with your own free Cloudflare Worker.

1. Go to [workers.cloudflare.com](https://workers.cloudflare.com) and create a free account — no credit card needed
2. Click **Workers & Pages** → **Create** → **Create Worker** → click **Deploy**
3. Click **Edit Code**, select all (Ctrl+A), delete and paste the worker code from the app's setup guide
4. Click **Deploy** and copy your Worker URL
5. Open the app, go to **Instellingen**, paste your Worker URL and save

Your Worker URL is saved in your browser — you only need to set it up once.

---

## How it works

```
Browser (your computer)
    │
    ▼
Cloudflare Worker (your free worker — optional but recommended)
    │
    ▼
Yahoo Finance API → real-time price, volume and candle data
    │
    ▼
VSA calculations → signals, VWAP, EMA, ATR, CVD
    │
    ▼
Results displayed in browser
```

No data is stored anywhere. Everything runs locally in your browser. Your settings are saved in localStorage.

---

## Tech Stack

| Component | Technology |
|---|---|
| Frontend | Vanilla HTML / CSS / JavaScript |
| Backend | Cloudflare Workers (free tier) |
| Market data | Yahoo Finance API |
| Hosting | GitHub Pages |

No frameworks, no build tools, no dependencies. Works in any modern browser.

---

## Related Tools

| Tool | Description | Link |
|---|---|---|
| 📡 **Gap Scanner** | Find momentum stocks daily using the Ross Cameron strategy | [goldminey-hub.github.io/gap-scanner](https://sahadataly.github.io/gap-scanner/) |

Both tools are free, open source and built for European traders.

---

## YouTube

Step-by-step tutorials in Dutch are available on the **GoldMineY** YouTube channel. Learn how to read VSA signals, set up the tool and apply the strategy in real market conditions.

---

## Disclaimer

This tool is for **educational purposes only**. Trading involves risk. You can lose (part of) your investment. Past performance is not indicative of future results. This is not financial advice.

---

## License

MIT — free to use, modify and distribute.
