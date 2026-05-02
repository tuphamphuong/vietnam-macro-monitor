# Vietnam Macro Risk Monitor

> Sovereign Risk Terminal v3.3 · 68 indicators · Live APIs · Telegram alerts

A single-file HTML dashboard tracking Vietnam's macroeconomic risks with real-time data feeds, BIS-framework early warning system, and Stagflation Composite Index.

## 🚀 Features

- **68 macro indicators** across 10 categories (inflation, production, housing, fiscal, monetary, labor, external, corporate, global)
- **Crisis Early Warning System** following BIS framework (AUROC 0.83–0.85)
- **Stagflation Composite Index** — CPI + PMI + PPI aggregate
- **9 live API feeds** (USD/VND, DXY, US10Y, Brent Oil, VIX, CNY/USD, S&P 500, Nikkei, Bitcoin) refreshing every 60s
- **Telegram Bot alerts** with deduplication and daily digest
- **Policy Effectiveness Tracker** — 6 major policies with 24 KPIs
- **Bank watchlist** — 10 banks by real estate exposure
- **Zero backend** — single HTML file, runs on any static host

## 🌐 Live Demo

After enabling GitHub Pages, dashboard will be accessible at:
```
https://<your-username>.github.io/<repo-name>/
```

## 🛠️ Tech Stack

- Pure vanilla JavaScript (no frameworks)
- Chart.js 4.4.0 (via CDN)
- Google Fonts: Fraunces, JetBrains Mono, Inter Tight
- Fetch APIs: Yahoo Finance (via corsproxy.io), CoinGecko, Fawazahmed Currency

## 📱 Telegram Alerts Setup

1. Create bot via [@BotFather](https://t.me/BotFather) → `/newbot`
2. Get Chat ID from [@userinfobot](https://t.me/userinfobot)
3. Click **⚙ TELEGRAM ALERTS** button in dashboard → paste credentials → Save & Test

Credentials are stored locally in browser (localStorage only).

## 🔄 Data Update Schedule

Vietnamese macro data requires manual update (no public APIs):

| Frequency | What to update |
|---|---|
| Monthly (6th) | CPI, Core CPI, Food inflation (NSO) |
| Monthly (2-3rd) | Manufacturing PMI (S&P Global) |
| Monthly | Credit growth, M2 (NHNN) |
| Quarterly | Property prices (Savills/CBRE), GDP, BoP |
| Quarterly | Household/Corporate debt ratios |

Edit `STATIC_DATA.extended.*` and `STATIC_DATA.coreMetrics` in index.html.

## 🔐 Privacy

- Telegram bot token stored only in your browser's localStorage
- No server-side tracking or analytics
- All API calls made directly from your browser to public endpoints

## 📄 License

Educational framework · Not investment advice · MIT-style permissive use

---

Built with Claude
