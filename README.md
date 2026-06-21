# Sphere (sphere-tax)

Sphere is a developer-first global indirect tax compliance platform that automates sales tax, VAT, and GST across nexus monitoring, registration, real-time calculation, and filing/remittance. Its REST API lets billing and checkout flows call the Sphere tax engine to calculate tax on transactions and export transaction data, authenticated with an X-API-KEY header.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/sphere-tax/refs/heads/main/apis.yml)

> Disambiguation: this repo documents **Sphere at getsphere.com**, the AI-powered sales-tax / VAT / GST compliance company. It is not Sphere Commerce/Payments, Sphere healthcare payments, any "Sphere" crypto/Web3 project, Microsoft Azure Sphere, or Sphere Engine. See `review.yml` for details.

## Tags

- Tax
- Sales Tax
- VAT
- GST
- Compliance
- FinTech

## Timestamps

- **Created:** 2026-06-21
- **Modified:** 2026-06-21

## APIs

### Sphere Tax Calculations API

Real-time indirect tax calculation for billing and checkout flows. POST line items, a customer address, and a currency to /tax_api/calculate_tax and receive per-line tax amounts, taxable amounts, and rate breakdown (jurisdiction, country, state, tax type).

- **Human URL:** [https://docs.getsphere.com/features/integrations/api/tax-calculation](https://docs.getsphere.com/features/integrations/api/tax-calculation)
- **Base URL:** `https://server.getsphere.com`

#### Tags

- Tax
- Calculation
- Sales Tax

#### Properties

- [Documentation](https://docs.getsphere.com/features/integrations/api/tax-calculation)
- [API Reference](https://docs.getsphere.com/features/integrations/api)
- [OpenAPI](openapi/sphere-tax-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sphere-tax.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sphere-tax.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sphere Transactions Export API

Asynchronous export of transaction data for reporting and reconciliation. Create an export job, poll its status, retrieve the download, or cancel a running job via the /tax_api/exports endpoints.

- **Human URL:** [https://docs.getsphere.com/features/reports/transaction-export](https://docs.getsphere.com/features/reports/transaction-export)
- **Base URL:** `https://server.getsphere.com`

#### Tags

- Transactions
- Export
- Reporting

#### Properties

- [Documentation](https://docs.getsphere.com/features/reports/transaction-export)
- [API Reference](https://docs.getsphere.com/features/integrations/api)
- [OpenAPI](openapi/sphere-tax-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/sphere-tax.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/sphere-tax.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Sphere Registrations and Filings API

Registration in tax jurisdictions globally and automated filing and remittance are delivered as Sphere platform features. No dedicated public REST endpoints for registration or filing are documented in the public API reference as of this writing; these are managed through the Sphere app and prebuilt connectors.

- **Human URL:** [https://docs.getsphere.com/features/registration](https://docs.getsphere.com/features/registration)
- **Base URL:** `https://server.getsphere.com`

#### Tags

- Registration
- Filing
- Remittance

#### Properties

- [Documentation](https://docs.getsphere.com/features/registration)
- [Documentation](https://docs.getsphere.com/features/filing-and-remittance)
- [OpenAPI](openapi/sphere-tax-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Sphere Nexus Monitoring API

Monitoring tracks global tax exposure and nexus thresholds so teams can plan for compliance. Surfaced as a Sphere platform feature; no dedicated public REST endpoint for nexus monitoring is documented in the public API reference.

- **Human URL:** [https://docs.getsphere.com/features/monitoring](https://docs.getsphere.com/features/monitoring)
- **Base URL:** `https://server.getsphere.com`

#### Tags

- Nexus
- Monitoring
- Exposure

#### Properties

- [Documentation](https://docs.getsphere.com/features/monitoring)
- [OpenAPI](openapi/sphere-tax-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Sphere Exemptions API

Exemption handling is applied within Sphere's calculation engine. No dedicated public REST endpoint for managing exemptions or exemption certificates is documented in the public API reference; exemption behavior is reflected in calculate_tax results.

- **Human URL:** [https://docs.getsphere.com/features/calculation](https://docs.getsphere.com/features/calculation)
- **Base URL:** `https://server.getsphere.com`

#### Tags

- Exemptions
- Tax Exempt
- Certificates

#### Properties

- [Documentation](https://docs.getsphere.com/features/calculation)
- [OpenAPI](openapi/sphere-tax-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

### Sphere Webhooks API

Sphere markets RESTful APIs and webhooks for integration with billing systems and ERPs. A specific webhook event catalog and subscription endpoints are not detailed in the public API reference as of this writing; webhook delivery is configured via integrations and prebuilt connectors.

- **Human URL:** [https://docs.getsphere.com/features/integrations](https://docs.getsphere.com/features/integrations)
- **Base URL:** `https://server.getsphere.com`

#### Tags

- Webhooks
- Events
- Notifications

#### Properties

- [Documentation](https://docs.getsphere.com/features/integrations)
- [OpenAPI](openapi/sphere-tax-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)

## Authentication

The Sphere API authenticates with an API key supplied in the **`X-API-KEY`** request header against the base URL `https://server.getsphere.com`. (Note: Sphere uses `X-API-KEY`, not a Bearer `Authorization` header.) Contact the Sphere team to obtain an API key.

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/getsphere)
- [Website](https://www.getsphere.com/)
- [Documentation](https://docs.getsphere.com/)
- [Plans](plans/sphere-tax-plans-pricing.yml)
- [Rate Limits](rate-limits/sphere-tax-rate-limits.yml)
- [Fin Ops](finops/sphere-tax-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
