---
name: basiq-onboard-user
description: Authenticate to Basiq, create a user, and track the connection job (including MFA) that links their bank.
api: Basiq API
operations:
- postToken
- createUser
- getUser
- getUserJobs
- getJobs
- postJobMfa
generated: '2026-10-21'
method: generated
---

# basiq-onboard-user

Base URL: https://au-api.basiq.io. MCP: https://api.basiq.io/mcp (generic execute-request tool).

1. `postToken` (POST /token) with `Authorization: Basic <API key>`, header `basiq-version: 3.0`, form body `scope=SERVER_ACCESS`. Use the returned JWT as `Authorization: Bearer` (services_token) on every other call.
2. `createUser` (POST /users) returns the user id. `getUser` reads it back.
3. Bank linking happens in Basiq's consent flow using a `CLIENT_ACCESS` token (`postToken` with `scope=CLIENT_ACCESS` and `userId`); see https://api.basiq.io/docs.
4. Poll `getUserJobs` (GET /users/{userId}/jobs) then `getJobs` (GET /jobs/{jobId}) until the steps complete.
5. If a job step requires MFA, submit it with `postJobMfa` (POST /jobs/{jobId}/mfa); the spec says this needs a CLIENT_ACCESS token with basiq-version 3.0. Expect 202.
