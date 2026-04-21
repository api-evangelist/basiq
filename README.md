# Basiq (basiq)
Basiq is an Australian open banking and financial data API platform providing unified access to bank account data and enrichment services. It enables fintechs, lenders, and financial service providers to connect to 180+ Australian and New Zealand banks via CDR (Consumer Data Right) and third-party connectors.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Australia, Banking, CDR, Financial Data, Fintech, Open Banking, Transactions

## Timestamps

- **Created:** 2026-03-27
- **Modified:** 2026-04-19

## APIs

### Basiq API
Open banking API providing user management, bank connections, account balances, transaction history, income verification, and expense categorization for Australian and New Zealand banks.

**Human URL:** [https://api.basiq.io/reference](https://api.basiq.io/reference)

#### Properties

- [Documentation](https://api.basiq.io/reference)
- [Getting Started](https://api.basiq.io/reference/getting-started)
- [OpenAPI](openapi/basiq-api-openapi.yml)

## Common Properties

- [Website](https://basiq.io/)
- [API Reference](https://api.basiq.io/reference)
- [Developer Dashboard](https://dashboard.basiq.io/)
- [GitHub Organization](https://github.com/basiqio)
- [Terms of Use](https://basiq.io/legal/terms-of-use/)
- [Privacy Policy](https://basiq.io/legal/privacy-policy/)

## Features

| Name | Description |
|------|-------------|
| Bank Connections | Connect to 180+ Australian and New Zealand banks via CDR and third-party connectors. |
| Account Data | Retrieve real-time account balances, available funds, and account metadata. |
| Transaction History | Access enriched transaction history with categorization and merchant data. |
| Income Verification | Automated income stream identification and regular/irregular income calculation. |
| Expense Categorization | Transaction-based expense categorization for affordability and budgeting analysis. |
| CDR Compliance | Consumer Data Right (CDR) compliant data access for Australian open banking. |
| Data Enrichment | Transaction enrichment with merchant names, categories, and subcategories. |

## Use Cases

| Name | Description |
|------|-------------|
| Lending and Credit Assessment | Use income verification and expense data to assess creditworthiness and affordability. |
| Personal Finance Apps | Aggregate bank accounts and transactions for budgeting and financial planning tools. |
| Mortgage Applications | Automate bank statement verification and income confirmation for home loan applications. |
| BNPL Affordability | Assess buy-now-pay-later affordability using real-time transaction and income data. |
| Financial Advisory | Provide financial planners with complete client financial pictures across institutions. |
| Account Verification | Verify bank account ownership for payment and identity verification workflows. |

## Artifacts

### OpenAPI

- [Basiq API](openapi/basiq-api-openapi.yml)

### JSON-LD

- [Basiq JSON-LD Context](json-ld/basiq-context.jsonld)

## Capabilities

### Shared Per-API Definitions

- [Basiq API](capabilities/shared/basiq-api.yaml) — 11 key operations

### Workflow Capabilities

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Open Banking](capabilities/open-banking.yaml) | Basiq | 7 | Fintech Developer, Lender, Financial Planner |

## Vocabulary

- [Basiq Vocabulary](vocabulary/basiq-vocabulary.yaml) — 6 resources, 4 actions, 1 workflow, 3 personas

## Rules

- [Basiq Spectral Rules](rules/basiq-spectral-rules.yml) — 15 rules enforcing API conventions

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
