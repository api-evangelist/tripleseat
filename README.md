# Tripleseat (tripleseat)

Tripleseat is event management and catering sales software for restaurants, hotels, and unique venues, helping operators capture leads, book events, and manage the sales lifecycle. Tripleseat provides a public REST API and webhooks for partners and customers to integrate event and lead data with external systems. The API exposes endpoints for leads, events, accounts, contacts, locations, sites, and users, and supports a public lead form for capturing inquiries directly into Tripleseat. Webhooks emit trigger events such as CREATE_LEAD, CONVERT_LEAD, and CONVERT_LEAD_TO_BOOKING, signed with a SHA256-HMAC X-Signature header. Authentication moved from OAuth 1.0 to OAuth 2.0, with OAuth 1.0 discontinued on July 1, 2026, and v1 endpoints served from api.tripleseat.com.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/apis.yml)

## Scope

- **Type:** Index

## Tags

- Restaurant
- Events
- Catering
- Leads
- Webhooks
- Sales

## Timestamps

- **Created:** 2026-06-02
- **Modified:** 2026-06-03

## APIs

### Tripleseat API

The Tripleseat REST API provides access to leads, events, accounts, contacts, locations, sites, and users for event and catering sales workflows. A public lead form endpoint captures inquiries directly into Tripleseat, and webhooks emit events such as CREATE_LEAD, CONVERT_LEAD, and CONVERT_LEAD_TO_BOOKING to subscriber URLs. The API uses OAuth 2.0 authentication, paginates 50 records per page via the page parameter, enforces a 10 requests-per-second limit on leads and events endpoints, and is served from api.tripleseat.com under the v1 path.

- **Human URL:** [https://support.tripleseat.com/hc/en-us/articles/205162108-API-Overview](https://support.tripleseat.com/hc/en-us/articles/205162108-API-Overview)
- **Base URL:** `https://api.tripleseat.com`

#### Tags

- Leads
- Events
- Webhooks
- Accounts

#### Properties

- [Documentation](https://support.tripleseat.com/hc/en-us/articles/205162108-API-Overview)
- [Authentication](https://support.tripleseat.com/hc/en-us/articles/19394408627479-API-Authentication)
- [API Reference](https://support.tripleseat.com/hc/en-us/sections/200821727-Tripleseat-API)
- [OpenAPI](openapi/tripleseat-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/tripleseat.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/tripleseat.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/tripleseat-webhooks-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON Schema](json-schema/tripleseat-api-lead-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-lead-create-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-account-update-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-contact-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-contact-create-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-location-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-site-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-api-user-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-webhooks-webhook-payload-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/tripleseat-webhooks-webhook-headers-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/tripleseat-api-lead-structure.json)
- [JSON Structure](json-structure/tripleseat-api-event-structure.json)
- [JSON Structure](json-structure/tripleseat-api-account-structure.json)
- [JSON Structure](json-structure/tripleseat-api-contact-structure.json)
- [JSON Structure](json-structure/tripleseat-api-lead-create-structure.json)
- [JSON Structure](json-structure/tripleseat-api-account-update-structure.json)
- [JSON Structure](json-structure/tripleseat-api-contact-create-structure.json)
- [JSON Structure](json-structure/tripleseat-api-location-structure.json)
- [JSON Structure](json-structure/tripleseat-api-site-structure.json)
- [JSON Structure](json-structure/tripleseat-api-user-structure.json)
- [JSON Structure](json-structure/tripleseat-webhooks-webhook-payload-structure.json)
- [JSON Structure](json-structure/tripleseat-webhooks-webhook-headers-structure.json)
- [JSON-LD](json-ld/tripleseat-api-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [JSON-LD](json-ld/tripleseat-webhooks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Example](examples/tripleseat-api-lead-example.json)
- [Example](examples/tripleseat-api-event-example.json)
- [Example](examples/tripleseat-api-account-example.json)
- [Example](examples/tripleseat-api-contact-example.json)
- [Example](examples/tripleseat-api-lead-create-example.json)
- [Example](examples/tripleseat-api-account-update-example.json)
- [Example](examples/tripleseat-api-contact-create-example.json)
- [Example](examples/tripleseat-api-location-example.json)
- [Example](examples/tripleseat-api-site-example.json)
- [Example](examples/tripleseat-api-user-example.json)
- [Example](examples/tripleseat-webhooks-webhook-payload-example.json)
- [Example](examples/tripleseat-webhooks-webhook-headers-example.json)

## Common Properties

- [Website](https://tripleseat.com)
- [Documentation](https://support.tripleseat.com/hc/en-us/sections/200821727-Tripleseat-API)
- [Support](https://support.tripleseat.com/hc/en-us)
- [GitHub Organization](https://github.com/tripleseat)
- [Blog](https://tripleseat.com/blog/)
- [Marketplace](https://tripleseat.com/partnermarketplace/)
- [Partners](https://tripleseat.com/partner-types/integrations/)
- [Pricing](https://support.tripleseat.com/hc/en-us/sections/24155934375191-Registration-and-Pricing)
- [LinkedIn](https://www.linkedin.com/company/tripleseat-software/)
- [Spectral Rules](rules/tripleseat-spectral-rules.yml)
- [Vocabulary](vocabulary/tripleseat-vocabulary.yaml)
- [Plans](plans/tripleseat-plans-pricing.yml)
- [Rate Limits](rate-limits/tripleseat-rate-limits.yml)
- [Fin Ops](finops/tripleseat-finops.yml)
- [Features](undefined)
- [Use Cases](undefined)
- [Integrations](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
