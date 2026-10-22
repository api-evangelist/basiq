---
name: basiq-read-financial-data
description: Read a connected user's accounts and transactions.
api: Basiq API
operations:
- getAccounts
- getAccount
- getTransactions
- getTransaction
generated: '2026-10-21'
method: generated
---

# basiq-read-financial-data

Base URL: https://au-api.basiq.io. MCP: https://api.basiq.io/mcp (generic execute-request tool).

1. Get a SERVER_ACCESS token with `postToken` first (see basiq-onboard-user).
2. `getAccounts` (GET /users/{userId}/accounts), then `getAccount` for detail.
3. `getTransactions` (GET /users/{userId}/transactions) supports `limit` and `filter` query parameters; `getTransaction` for one item.
4. All reads are safe GETs; 403/404 mean the token or userId is wrong; 503 on getTransaction is retryable.
