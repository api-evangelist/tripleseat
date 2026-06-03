# Tripleseat (tripleseat)
Tripleseat is event management and catering sales software for restaurants, hotels, and unique venues, helping operators capture leads, book events, and manage the sales lifecycle. Tripleseat provides a public REST API and webhooks for partners and customers to integrate event and lead data with external systems. The API exposes endpoints for leads, events, accounts, contacts, locations, sites, and users, and supports a public lead form for capturing inquiries directly into Tripleseat. Webhooks emit trigger events such as CREATE_LEAD, CONVERT_LEAD, and CONVERT_LEAD_TO_BOOKING, signed with a SHA256-HMAC X-Signature header. Authentication moved from OAuth 1.0 to OAuth 2.0, with OAuth 1.0 discontinued on July 1, 2026, and v1 endpoints served from api.tripleseat.com.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/tripleseat/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Restaurant, Events, Catering, Leads, Webhooks, Sales

## Timestamps

- **Created:** 2026-06-02
- **Modified:** 2026-06-03

## APIs

### Tripleseat API
The Tripleseat REST API provides access to leads, events, accounts, contacts, locations, sites, and users for event and catering sales workflows. A public lead form endpoint captures inquiries directly into Tripleseat, and webhooks emit events such as CREATE_LEAD, CONVERT_LEAD, and CONVERT_LEAD_TO_BOOKING to subscriber URLs. The API uses OAuth 2.0 authentication, paginates 50 records per page via the page parameter, enforces a 10 requests-per-second limit on leads and events endpoints, and is served from api.tripleseat.com under the v1 path.

**Human URL:** [https://support.tripleseat.com/hc/en-us/articles/205162108-API-Overview](https://support.tripleseat.com/hc/en-us/articles/205162108-API-Overview)

**Base URL:** https://api.tripleseat.com

#### Tags:

 - Leads, Events, Webhooks, Accounts

#### Properties

- [Documentation](https://support.tripleseat.com/hc/en-us/articles/205162108-API-Overview)
- [Authentication](https://support.tripleseat.com/hc/en-us/articles/19394408627479-API-Authentication)
- [APIReference](https://support.tripleseat.com/hc/en-us/sections/200821727-Tripleseat-API)
- [OpenAPI](openapi/tripleseat-openapi.yml)
- [AsyncAPI](asyncapi/tripleseat-webhooks-asyncapi.yml)

## Common Properties

- [Website](https://tripleseat.com)
- [Documentation](https://support.tripleseat.com/hc/en-us/sections/200821727-Tripleseat-API)
- [Support](https://support.tripleseat.com/hc/en-us)
- [GitHubOrganization](https://github.com/tripleseat)
- [Blog](https://tripleseat.com/blog/)
- [Marketplace](https://tripleseat.com/partnermarketplace/)
- [Partners](https://tripleseat.com/partner-types/integrations/)
- [Pricing](https://support.tripleseat.com/hc/en-us/sections/24155934375191-Registration-and-Pricing)
- [LinkedIn](https://www.linkedin.com/company/tripleseat-software/)
- [SpectralRules](rules/tripleseat-spectral-rules.yml)
- [Vocabulary](vocabulary/tripleseat-vocabulary.yaml)
- [Plans](plans/tripleseat-plans-pricing.yml)
- [RateLimits](rate-limits/tripleseat-rate-limits.yml)
- [FinOps](finops/tripleseat-finops.yml)

## Features

| Name | Description |
|------|-------------|
| Lead Capture | Capture inquiries through the public lead form API and the leads endpoints, routing leads to the correct location. |
| Event And Booking Management | Retrieve and manage events and bookings across the sales lifecycle. |
| Account And Contact CRM | Maintain accounts and their associated contacts for customer records. |
| Webhooks | Subscribe to lead and booking lifecycle events, verified with a SHA256-HMAC X-Signature header. |
| Multi-Location Support | Model sites that group multiple locations and target leads and events at specific locations. |

## Use Cases

| Name | Description |
|------|-------------|
| Website Lead Forms | Embed a public lead form on a website to push inquiries directly into Tripleseat via the lead form API. |
| CRM And Marketing Sync | Synchronize accounts, contacts, and events with external CRM and email marketing platforms. |
| Real-Time Integrations | React to lead creation and conversion in real time using webhooks to drive downstream automation. |
| Reporting And Analytics | Extract events and leads into data warehouses and dashboards for sales reporting. |

## Integrations

| Name | Description |
|------|-------------|
| SevenRooms | Reservation, seating, and guest management platform that shares reservation and event details with Tripleseat. |
| OpenTable Guest Center | Connect Tripleseat events to OpenTable guest center bookings to avoid double bookings. |
| Tock | Collect private event leads from Tock and transfer them into Tripleseat. |
| Square | Tripleseat integration available through the Square App Marketplace. |

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Tripleseat API](openapi/tripleseat-openapi.yml)

### AsyncAPI

- [Tripleseat Webhooks](asyncapi/tripleseat-webhooks-asyncapi.yml)

### JSON Schema

- [Lead](json-schema/tripleseat-api-lead-schema.json)
- [Lead Create](json-schema/tripleseat-api-lead-create-schema.json)
- [Event](json-schema/tripleseat-api-event-schema.json)
- [Account](json-schema/tripleseat-api-account-schema.json)
- [Account Update](json-schema/tripleseat-api-account-update-schema.json)
- [Contact](json-schema/tripleseat-api-contact-schema.json)
- [Contact Create](json-schema/tripleseat-api-contact-create-schema.json)
- [Location](json-schema/tripleseat-api-location-schema.json)
- [Site](json-schema/tripleseat-api-site-schema.json)
- [User](json-schema/tripleseat-api-user-schema.json)
- [Webhook Payload](json-schema/tripleseat-webhooks-webhook-payload-schema.json)
- [Webhook Headers](json-schema/tripleseat-webhooks-webhook-headers-schema.json)

### JSON Structure

- 12 JSON Structure files in [json-structure/](json-structure/) mirroring the JSON Schema models.

### JSON-LD

- [Tripleseat API Context](json-ld/tripleseat-api-context.jsonld)
- [Tripleseat Webhooks Context](json-ld/tripleseat-webhooks-context.jsonld)

### Examples

- 12 example payloads in [examples/](examples/) for the core resources and webhook payloads.

## Capabilities

Naftiko capabilities organized as self-contained, per-business-surface definitions, each exposing one REST adapter and one MCP adapter.

| Workflow | APIs Combined | Tools | Persona |
|----------|--------------|-------|---------|
| [Leads](capabilities/tripleseat-leads.yaml) | Tripleseat API | 4 | Sales Manager, Integration Developer |
| [Events](capabilities/tripleseat-events.yaml) | Tripleseat API | 3 | Sales Manager, Operations Coordinator |
| [Accounts](capabilities/tripleseat-accounts.yaml) | Tripleseat API | 3 | Sales Manager |
| [Contacts](capabilities/tripleseat-contacts.yaml) | Tripleseat API | 1 | Sales Manager |
| [Locations](capabilities/tripleseat-locations.yaml) | Tripleseat API | 1 | Operations Coordinator |
| [Sites](capabilities/tripleseat-sites.yaml) | Tripleseat API | 1 | Operations Coordinator |
| [Users](capabilities/tripleseat-users.yaml) | Tripleseat API | 2 | Administrator |

## Vocabulary

- [Tripleseat Vocabulary](vocabulary/tripleseat-vocabulary.yaml) — Unified taxonomy mapping 7 resources, 5 actions, 7 workflows, and 4 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Tripleseat Spectral Rules](rules/tripleseat-spectral-rules.yml) — 33 rules across 13 categories enforcing Tripleseat API conventions.

## Plans, Rate Limits & FinOps

- [Plans & Pricing](plans/tripleseat-plans-pricing.yml) — Custom-quoted per-venue annual subscription with optional add-ons and Floorplans memberships (API Commons Plans 0.1).
- [Rate Limits](rate-limits/tripleseat-rate-limits.yml) — 10 requests per second on leads and events endpoints; 50-record pagination; webhook retry policy (API Commons Rate Limits 0.1).
- [FinOps](finops/tripleseat-finops.yml) — FOCUS-aligned subscription billing model (FinOps Framework 1.0).

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
