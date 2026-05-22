# Portfolio Tracker

A mobile-first investment portfolio tracker for stock transactions, supporting multiple owners with configurable share percentages.

## Features

- **Multi-owner support** — Track investments across multiple people (Murat, Yusuf, Cüneyt) with configurable % splits
- **Transaction types** — Buy, Sell, Deposit, Withdraw
- **$1.50 per-transaction fee** — Automatically added to buy cost, deducted from sell revenue
- **Partial/multiple transactions** — Set number of partial fills to multiply the fee count
- **FIFO P&L calculation** — Realized P&L calculated using First-In-First-Out method
- **Per-owner view** — Filter all views by owner
- **Stock view** — Open and closed positions with average cost and P&L
- **Transaction log** — Full history with delete capability
- **CSV Export** — Download your full transaction history
- **Local storage** — Data persists in your browser automatically

## Access on iPhone

Visit: **`https://YOUR_GITHUB_USERNAME.github.io/portfolio-tracker/`**

Save to home screen:
1. Open in Safari
2. Tap the Share button (box with arrow)
3. Tap "Add to Home Screen"
4. Tap "Add"

## Deploy to GitHub Pages

1. Create a new GitHub repository named `portfolio-tracker`
2. Upload `index.html` to the repository
3. Go to Settings → Pages → Source: Deploy from branch → main → / (root)
4. Wait ~1 minute, then visit `https://YOUR_USERNAME.github.io/portfolio-tracker/`

## Transaction Fee Logic

- Each transaction (buy or sell) has a **$1.50 cost**
- For **buys**: fee is **added** to the cost basis
- For **sells**: fee is **deducted** from the revenue
- For **partial fills** (multiple broker orders for one position): set "Number of Partial Transactions" to multiply the fee

## Owner Shares

Each trade can be split across owners in any percentage. Percentages must sum to 100%. Quick presets:
- Equal split
- Custom (e.g. 88.6% / 8.2% / 3.2% matching your Excel)

## Data

All data is stored in your browser's `localStorage`. Use "Export CSV" to back up your data regularly.
