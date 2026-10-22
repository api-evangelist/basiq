---
name: basiq-manage-connections-and-consent
description: Refresh, delete or purge bank connections and revoke a user's consent.
api: Basiq API
operations:
- getConnections
- getConnection
- refreshConnection
- refreshConnections
- deleteConnection
- purgeConnectionData
- getConsents
- deleteConsent
- deleteUser
generated: '2026-10-21'
method: generated
---

# basiq-manage-connections-and-consent

Base URL: https://au-api.basiq.io. MCP: https://api.basiq.io/mcp (generic execute-request tool).

1. `getConnections` / `getConnection` to inspect connections.
2. `refreshConnection` or `refreshConnections` returns 202 and starts a job; track it with `getJobs`.
3. `getConsents` lists consents; `deleteConsent` revokes one (204).
4. Destructive and irreversible: `deleteConnection`, `purgeConnectionData`, `deleteUser` (all 204). Confirm with a human before calling. The specs document no idempotency keys, so do not blindly retry POST refreshes.
