# PromptQL - AML Project

This project uses Hasura PromptQL to build a conversational AI system over two real-time financial data sources: **PostgreSQL** and **MongoDB**. It allows natural language querying and actions over AML (Anti-Money Laundering) datasets.

## 📊 Data Sources

### 🔹 PostgreSQL (`aml_postgres`)
- Customers: PEP/blacklist, jurisdiction, risk tier
- Transfers: sender/receiver, volumes, indicators, currencies
- SARs: narratives, tags, filing status

### 🔹 MongoDB (`aml_mongo`)
- Accounts: risk level, contact info, entity type, txn limits
- AML Cases: flags, volumes, counterparties, statuses
- Sanctions: sanctioned entities, addresses, programs, countries

## 🚀 Setup Instructions

> These are the local development steps, assuming Docker, DDN CLI, and SSH tunnel are set up.

```bash
ddn run docker-start      # Start local engine
ddn console --local       # Open PromptQL Playground

