# Engineering Portfolio

Three ongoing software projects spanning full-stack commerce, property and accounting workflows, and AI-assisted document processing. Each case study explains the implemented architecture, engineering challenges, test scenarios and current limits.

## Projects

| Project | What it does | Engineering focus | Current state |
| --- | --- | --- | --- |
| [LUCA](case-studies/luca.md) | Product discovery, guest checkout, delivery/pickup and administration | Transactional orders, duplicate-request handling, payment coordination and media processing | Ongoing application; production acceptance unverified |
| [Property Management & Accounting System](case-studies/property-management-accounting.md) | Connects property and agreement management with billing, receipts, payables and reporting | Modular backend, concurrent commands, audit events and company context | Ongoing application; production identity integration incomplete |
| [Invoice Extraction & Review Workbench](case-studies/invoice-converter.md) | Converts selected invoice pages into reviewable structured drafts | Vision-model integration, deterministic validation, source evidence and revisioned corrections | Local prototype; review JSON download implemented; accounting export remains future work |

## Technologies

- **LUCA:** Next.js, React, TypeScript, Prisma, PostgreSQL, Better Auth, HitPay, Sharp and S3-compatible object storage.
- **Property and accounting:** Next.js, React, TypeScript, NestJS, Prisma and PostgreSQL.
- **Invoice processing:** Python, PDF rendering, an OpenAI-compatible vision adapter, Starlette, HTTPX and a browser review interface.

## Engineering themes

- **Transaction boundaries:** coordinating database state with payment providers and concurrent business operations.
- **Explicit failure states:** handling retries, repeated requests, incomplete extraction and conflicting edits.
- **Traceability:** retaining order snapshots, audit events, original document observations and correction provenance.
- **Testing across layers:** unit, integration, database, concurrency and UI test scenarios in the private project repositories.

## Evidence and scope

The case studies reflect source inspection as of **29 October 2026**. “Implemented” describes code present in the inspected projects. Tests and evaluation tooling are identified where present; their current outcomes, live integrations and deployments have not been verified for this portfolio.

This repository contains documentation and architecture diagrams. Private source code, credentials, business records and proprietary rules remain outside it. Screenshots will be added only after review using synthetic data. No unmeasured business improvements or model-performance results are claimed.
