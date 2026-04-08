# Audit1

Insurance premium automation platform.

## Stack

- **Frontend**: Next.js 15, React 19, Tailwind CSS, Apollo Client
- **Backend**: TypeScript (Hono), Python (Flask), GraphQL (type-graphql)
- **Infrastructure**: Google Cloud Run, MongoDB Atlas, GCS

## Portals

| Portal | Description |
|--------|-------------|
| Admin | Internal operations dashboard |
| Carrier | Carrier-facing portal |
| Employer | Employer-facing portal (white-label) |
| Payroll Company | Payroll provider portal |

## Architecture

- **48 microservices** on Google Cloud Run
- **GraphQL gateway** with downstream CRUD and domain services
- **Ingestion pipeline**: SFTP, Connectors, Webhooks, Manual Upload, MCP
- **Validation engine**: Class code matching, wage calculation, premium computation
- **Shared UI library** (UI-Commons) across all portals
