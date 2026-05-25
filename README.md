# 📈 Portfolio Tracker

A fast, privacy-first investment portfolio tracker that runs entirely in your browser —
no account, no server, no data ever leaves your device.

🌐 **Live:** https://portfolio-tracker-cpen.netlify.app

---

## Overview

Portfolio Tracker lets you monitor your stocks, ETFs, and crypto across major North American
exchanges in real time. Built as a single HTML file with no backend, everything is stored
locally in your browser using localStorage.

---

## Features

### Core tracking
- Live prices fetched via Yahoo Finance (NYSE, NASDAQ, TSX, TSXV)
- Real-time CAD/USD conversion with live FX rate
- 52-week high/low range bar per holding
- Day change and total gain/loss columns
- CAGR (compound annual growth rate) per position

### Portfolio management
- Add buy lots with dollar-cost averaging support
- Record sales with automatic FIFO cost basis deduction
- Log dividends per holding
- Multi-lot positions with individual lot breakdown
- Stale price warnings with manual refresh

### Charts & analytics
- Performance chart with 1D, YTD, 1M, 3M, 1Y and 5Y periods
- SPY benchmark overlay to compare against the S&P 500
- Portfolio-wide combined return line
- Sector allocation breakdown
- Top gainers and losers panel

### Data & privacy
- All data stored in browser localStorage — nothing sent to any server
- Export to JSON (full backup) or CSV (spreadsheet-friendly)
- Import JSON to restore a previous backup
- No account required

---

## Tech Stack

| Layer | Details |
|---|---|
| Language | Vanilla JavaScript (no frameworks) |
| Charts | Chart.js 4.4.1 |
| Fonts | IBM Plex Sans & IBM Plex Mono |
| Hosting | Netlify (auto-deploy from GitHub) |
| Data | Yahoo Finance API via CORS proxy |
| Storage | Browser localStorage |

---

## Deployment

This project auto-deploys to Netlify on every push to the `main` branch.

To update the live site:
1. Edit `index.html`
2. Commit and push to `main`
3. Netlify deploys automatically within ~30 seconds

---

## License

This project is for personal use. All rights reserved.
