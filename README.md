# 9ledger — Compliance-First ERP with Intelligent Automation *(Closed Project)*

**9ledger** was a SaaS accounting and business management platform built for Hungarian small and medium-sized businesses (SMEs). The project is now closed and no longer actively developed.

### What It Was

9ledger combined a full-featured ERP system (Enterprise Resource Planning — software that manages core business processes like accounting, invoicing, and inventory) with an AI-powered automation layer called **Nexus Assistant**. The goal was to let businesses automate up to 90% of routine accounting work while keeping a human specialist in control of every final decision.

### Key Features

- **Full accounting suite** — general ledger, accounts payable/receivable, bank reconciliation, VAT reporting, and fixed assets, built to Hungarian regulatory standards with native NAV (tax authority) integration
- **Intelligent automation** — document OCR, automatic transaction classification, bank reconciliation suggestions, and journal entry recommendations powered by machine learning
- **Supervised approval workflow** — a mandatory three-step process (Input → Specialist Review → Output) ensured that automation only assisted, never replaced, human judgment
- **Multi-tenant architecture** — designed to serve both individual SMEs and accounting firms managing dozens of client companies from a single platform

### Technical Highlights

- **Backend:** .NET 8 / ASP.NET Core, C# 12, PostgreSQL 15, Entity Framework Core
- **Frontend:** React 18, TypeScript 5, Vite
- **Infrastructure:** Docker, GitHub Actions CI/CD, OpenTelemetry observability
- **Security:** OAuth 2.0/OIDC authentication, AES-256 encryption at rest, TLS 1.3 in transit, schema-based multi-tenant data isolation, immutable audit logs
- Designed to meet GDPR and SOC 2 compliance requirements

### My Contributions

Sole developer responsible for the full product lifecycle: architecture design, domain modelling (double-entry bookkeeping engine, approval workflows, multi-tenancy), frontend and backend implementation, business strategy, and customer-facing documentation.

### Outcomes & Learnings

- Designed and documented a production-grade accounting engine from first principles, including strict double-entry validation, immutable journal entries, and period-close locking
- Architected a clean separation between the automation layer and the core ERP, so the system remained fully functional with or without AI assistance
- Built an extensible, API-first platform capable of scaling from micro-businesses to mid-market firms and accounting practices
- Gained deep experience in compliance-driven software design, Hungarian accounting regulation, and the challenges of building trust in automated financial tooling
