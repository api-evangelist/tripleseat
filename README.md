# Tripleseat (tripleseat)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
