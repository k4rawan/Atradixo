# Atradixo — AI Trading Desk

An independent trading-desk build. This repository is separate from `karab-commits/trading-desk`; that project is not modified.

## Current status
This is a front-end prototype with a responsive dashboard, three virtual strategy sleeves, an eight-role AI specialist roster, sample signal generation, and a human review queue. It is **simulation-only**.

## Run
Open `index.html` in a browser, or enable GitHub Pages in repository Settings → Pages → Deploy from branch → `main` → `/ (root)`.

## Safety and limitations
- No broker or market-data connection is configured.
- Demo signals are illustrative, not live market data or investment advice.
- The approval queue only records a local simulated decision; it never sends an order.
- Live execution is disabled and must remain disabled until authenticated, per-order approval, risk validation, audit logging, and broker safeguards are implemented.

## Planned production work
1. Market-data adapters for US/Canadian stocks and ETFs, with freshness checks.
2. Eight independent research agents with evidence-backed structured outputs.
3. Separate day, swing, and long-term paper portfolios.
4. Backtesting with commissions, spread, slippage, survivorship-bias controls, and out-of-sample validation.
5. Persistent scanner/scheduler and database-backed trade journal.
6. Questrade read-only account/data integration before any order capability.
7. A hard approval gate bound to the exact symbol, side, quantity, limit price, account, risk result, and expiry of each proposed order.
8. Emergency kill switch and immutable audit trail.

Starting capital and risk settings shown in the UI are placeholders for simulation only.