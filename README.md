# Sysco (sysco)

Sysco is the global leader in selling, marketing, and distributing food products to restaurants, healthcare and educational facilities, lodging establishments, and other foodservice customers. Sysco operates the Sysco Shop ecommerce platform (US, Canada, Bahamas) backed by an Apollo GraphQL supergraph composed of domain subgraphs for ordering, product, pricing, delivery, and accounts. Programmatic access is partner/customer-gated through the login-only APIC Developer Portal and through traditional EDI (X12) trading-partner integration; Sysco does not publish a self-serve public developer API, OpenAPI specification, or open GitHub presence.

**URL:** [apis.yml](https://raw.githubusercontent.com/api-evangelist/sysco/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Food Distribution
- Food Service
- Supply Chain
- Fortune 100
- Wholesale

## Timestamps

- **Created:** 2026-05-03
- **Modified:** 2026-06-03

## API Access Reality

Sysco's foodservice capabilities are real, but they are **not exposed as a public, self-serve developer API**:

- **Apollo GraphQL supergraph** — Sysco Shop is powered by eight domain subgraphs (ordering, product, pricing, delivery, accounts) across orchestration, core services, and enterprise tiers.
- **APIC Developer Portal** ([apic-devportal.sysco.com](https://apic-devportal.sysco.com/)) — exists with multiple environments (STG, PERF, DEV, SBX, DIM) but is **login-gated**; no public OpenAPI spec, API reference, paths, or schemas are published.
- **EDI (X12)** — the dominant B2B integration path. Sysco publishes trading-partner EDI specifications (e.g. 810 Invoice, 816 Organizational Relationships, 820 Payment Order/Remittance Advice), serviced by networks such as Stedi, Cleo, TrueCommerce, and Orderful.
- **No public GitHub presence** — the `SyscoCorporation` org has zero public repositories; no SDKs, MCP servers, or Claude Code skills were found.

> The OpenAPI artifact in this repo is a **non-authoritative, illustrative model** of the documented capability domains. It is not a contract published by Sysco.

## APIs

### Sysco Food Distribution API

Sysco's food distribution capabilities (product catalog browsing, order management, delivery tracking, account management, and pricing) are exposed through an Apollo GraphQL supergraph powering the Sysco Shop ecommerce platform, plus EDI (X12) integration for trading partners. Access is gated behind customer/partner onboarding via the login-only APIC Developer Portal; Sysco publishes no public, self-serve OpenAPI specification or open API reference.

**Human URL:** [apic-devportal.sysco.com](https://apic-devportal.sysco.com/)

#### Tags

- Food Distribution
- Ordering
- Restaurant
- Supply Chain
- Product Catalog
- Delivery Tracking

#### Properties

- [Documentation](https://apic-devportal.sysco.com/)
- [Developer Portal](https://apic-devportal.sysco.com/)
- [Login](https://apic-devportal.sysco.com/)
- [Illustrative (Non-Authoritative) OpenAPI](openapi/sysco-food-distribution-api-openapi.yml)

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/sysco)
- [Website](https://www.sysco.com)
- [Developer Portal](https://apic-devportal.sysco.com/)
- [GitHub Org](https://github.com/SyscoCorporation)
- [GraphQL (Apollo case study)](https://www.apollographql.com/customers/sysco)
- [JSON-LD Context](json-ld/sysco-context.jsonld)
- [Vocabulary](vocabulary/sysco-vocabulary.yml)

## Features

- Sysco Shop Ecommerce Platform (US, Canada, Bahamas)
- Apollo GraphQL Supergraph with Eight Domain Subgraphs
- Product Catalog with 30+ Data Fields
- Real-Time Stock Status
- Order Management
- Delivery Tracking
- Contract Pricing
- Account Management
- EDI (X12) Trading-Partner Integration
- Partner/Customer-Gated APIC Developer Portal

## Use Cases

- Food Service Ordering Automation
- Product Catalog Integration
- Delivery Schedule Management
- Supply Chain Visibility
- ERP Integration
- Restaurant Management System Integration

## Integrations

| Name | Description |
|------|-------------|
| Apollo GraphQL | Eight domain subgraphs (ordering, product, pricing, delivery, accounts) powering Sysco Shop. |
| EDI | X12 EDI documents (810, 816, 820) exchanged with trading partners under Sysco's EDI specifications. |
| Stedi | Third-party EDI network with pre-built Sysco X12 integration. |
| Cleo | Third-party EDI integration provider for Sysco compliance. |
| TrueCommerce | Third-party Sysco EDI trading-partner integration. |
| Orderful | API-first EDI network with pre-codified Sysco trading-partner integration. |
| Portable | Sysco-to-PostgreSQL data connector. |

## Solutions

- Restaurant Technology Integration
- Healthcare Food Service
- Education Food Service
- Hospitality Supply Chain

## Artifacts

Machine-readable artifacts in this repo. The OpenAPI spec and the schema/example/JSON-LD artifacts derived from it are **illustrative models** of documented capability domains, not contracts published by Sysco.

### OpenAPI

- [Sysco Food Distribution API (illustrative)](openapi/sysco-food-distribution-api-openapi.yml)

### JSON Schema

- [Sysco Product Schema](json-schema/sysco-product-schema.json)

### JSON Structure

- [Sysco Product Structure](json-structure/sysco-product-structure.json)

### JSON-LD

- [Sysco Context](json-ld/sysco-context.jsonld)

### Examples

- [List Products Response](examples/sysco-food-distribution-api-listProducts-example.json)
- [Create Order Request/Response](examples/sysco-food-distribution-api-createOrder-example.json)

### Plans, Rate Limits & FinOps

- [Plans & Pricing](plans/sysco-plans-pricing.yml) — no public developer pricing; access via Sysco Shop accounts and customer-specific EDI/integration onboarding (Contact Sales).
- [Rate Limits](rate-limits/sysco-rate-limits.yml) — no public rate-limit documentation; terms negotiated per customer integration agreement.
- [FinOps](finops/sysco-finops.yml) — no public API billing surface; consumption is reflected on customer invoices, not metered API line items.

## Vocabulary

- [Sysco Vocabulary](vocabulary/sysco-vocabulary.yml) — foodservice and integration taxonomy (SUPC, Order Guide, Case, Contract Price, GTIN, Route, Sysco Shop, Subgraph, EDI/X12) across operational and capability dimensions.

## Rules

- [Sysco Rules](rules/sysco-rules.yml) — 13 Spectral rules enforcing Sysco API conventions.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
