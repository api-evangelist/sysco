# Sysco

Sysco is the global leader in selling, marketing, and distributing food products to restaurants, healthcare and educational facilities, lodging establishments, and other foodservice customers. Sysco's APIC Developer Portal provides REST APIs for product catalog browsing, order management, delivery tracking, account management, and pricing integration.

**Type:** Company (Fortune 100)
**Website:** [sysco.com](https://www.sysco.com)
**Developer Portal:** [apic-devportal.sysco.com](https://apic-devportal.sysco.com/)

## APIs

### Food Distribution API

The Sysco Food Distribution API provides programmatic access to Sysco's food distribution platform for product catalog browsing, order management, delivery tracking, account management, and pricing. Enables restaurants, food service operators, and partners to automate their food supply chain.

- **Documentation:** [apic-devportal.sysco.com](https://apic-devportal.sysco.com/)
- **OpenAPI:** [openapi/sysco-food-distribution-api-openapi.yml](openapi/sysco-food-distribution-api-openapi.yml)
- **Base URL:** `https://api.sysco.com`

| Method | Path | Summary |
|--------|------|---------|
| GET | /products | List Products |
| GET | /products/{productId} | Get Product |
| GET | /orders | List Orders |
| POST | /orders | Create Order |
| GET | /orders/{orderId} | Get Order |
| DELETE | /orders/{orderId} | Cancel Order |
| GET | /deliveries | List Deliveries |
| GET | /deliveries/{deliveryId} | Get Delivery |
| GET | /accounts | List Accounts |
| GET | /accounts/{accountId} | Get Account |
| GET | /pricing | List Pricing |

## Naftiko Capabilities

### Shared Definitions

| File | Description |
|------|-------------|
| [capabilities/shared/food-distribution-api.yaml](capabilities/shared/food-distribution-api.yaml) | Food Distribution API consumed definition |

### Workflow Capabilities

| Capability | Description | Tools |
|-----------|-------------|-------|
| [food-supply-chain.yaml](capabilities/food-supply-chain.yaml) | Unified food supply chain (products + orders + deliveries + pricing) | 8 tools |

## Artifacts

| Type | File |
|------|------|
| OpenAPI | [openapi/sysco-food-distribution-api-openapi.yml](openapi/sysco-food-distribution-api-openapi.yml) |
| Spectral Rules | [rules/sysco-rules.yml](rules/sysco-rules.yml) |
| JSON Schema | [json-schema/sysco-product-schema.json](json-schema/sysco-product-schema.json) |
| JSON Structure | [json-structure/sysco-product-structure.json](json-structure/sysco-product-structure.json) |
| JSON-LD Context | [json-ld/sysco-context.jsonld](json-ld/sysco-context.jsonld) |
| Vocabulary | [vocabulary/sysco-vocabulary.yml](vocabulary/sysco-vocabulary.yml) |

## Examples

| File | Description |
|------|-------------|
| [examples/sysco-food-distribution-api-listProducts-example.json](examples/sysco-food-distribution-api-listProducts-example.json) | List products response |
| [examples/sysco-food-distribution-api-createOrder-example.json](examples/sysco-food-distribution-api-createOrder-example.json) | Create order request/response |

## Features

- Product Catalog with 30+ Data Fields (SUPC, GTIN, Brand, Category, Storage Type)
- Real-Time Stock Status and Next Receive Dates
- Order Management with Up to 14 Months History
- Delivery Tracking with ETA
- Contract and List Pricing
- Account Management
- GraphQL API via Apollo
- Staging and Production Environments

## Use Cases

- Restaurant Technology Integration
- ERP and Order Management System Integration
- Food Service Supply Chain Automation
- Product Catalog Synchronization
- Delivery Schedule Management

## Maintainers

**FN:** API Evangelist
**Email:** info@apievangelist.com
