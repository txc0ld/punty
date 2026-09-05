# Punty

A profit and loss dashboard for Australian bookmaker accounts. Drop in your Sportsbet, TAB or other transaction exports and get cumulative P&L, monthly results, strike rate, breakdowns by sport, bet type and odds, a betting-time heatmap, funding habits, and a searchable transaction ledger.

Everything runs in the browser. Files are parsed locally and saved to that device's localStorage. Nothing is uploaded to a server.

## Use it

Open the hosted page, click **How to export** for per-bookmaker instructions, then drag your CSV or XLSX onto the page.

- **Sportsbet** transaction history exports are detected automatically.
- **TAB, Ladbrokes, Neds, bet365, PointsBet and others** open a one-time column mapping step.
- Overlapping exports are fine. Duplicate transactions are skipped by transaction ID.

## What it tracks

| Section | What it shows |
|---|---|
| Headline | Punting P&L, ROI on stakes, total staked and returned, strike rate, average stake, deposits, withdrawals, net funding, max drawdown |
| Bet With Mates | Tracked separately from your own punting. A settings toggle folds it into the headline if you want that |
| Cash outs | Counted as returns, listed in Funding and habits, shown as their own outcome in the ledger |
| Reconciliation | Opening balance plus every movement is checked against the closing balance on the statement |
| Charts | Cumulative P&L, monthly P&L, by sport, by bet type, by odds band, cash flow, when you bet |
| Ledger | Every row with the bet outcome worked out by pairing stakes with results by bet ID. Search, sort, filter, export |

## Run locally

It is a single `index.html`. Open it in a browser, or serve the folder with any static server.

## Deploy

Static site, no build step. Vercel: import the repo and deploy with the defaults.
