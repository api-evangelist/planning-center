# Planning Center (planning-center)

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Planning Center is a suite of church management software products - People, Services, Giving, Groups, Check-Ins, Calendar, Registrations, and Publishing - used by churches to organize their people, plan worship services, process online giving, run small groups, manage attendance and check-in, schedule facilities and events, handle event registrations, and publish sermons. Each product exposes a documented public REST API under a shared base host (`https://api.planningcenteronline.com`), authenticated with OAuth 2.0 or a Personal Access Token and returning data in the JSON:API 1.0 format. A Webhooks API delivers create/update/destroy events across the products. The APIs are free to use with a Planning Center account; each product is subscribed to separately.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/planning-center/refs/heads/main/apis.yml)

## Tags

- Church Management
- ChMS
- Faith
- Giving
- Events
- Scheduling
- People
- Nonprofit

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Planning Center People API

The system of record for people in a Planning Center account. Read and write people, their emails, addresses, phone numbers, households, field data, lists, forms, and workflows. This is the shared people directory that the other products reference.

- **Human URL:** [https://developer.planning.center/docs/#/apps/people](https://developer.planning.center/docs/#/apps/people)
- **Base URL:** `https://api.planningcenteronline.com/people/v2`

#### Tags

- People
- Contacts
- Households
- Workflows

#### Properties

- [Documentation](https://developer.planning.center/docs/)
- [API Reference](https://developer.planning.center/docs/#/apps/people)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Services API

Plan and schedule worship services. Manage service types, plans and their items, songs and arrangements, teams and team members, and the people scheduled to serve on each plan.

- **Human URL:** [https://developer.planning.center/docs/#/apps/services](https://developer.planning.center/docs/#/apps/services)
- **Base URL:** `https://api.planningcenteronline.com/services/v2`

#### Tags

- Services
- Worship
- Plans
- Scheduling

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/services)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Giving API

Read and write online and offline giving records - donations and their designations, funds, batches, payment sources, pledges, and recurring donations. Push gifts from an external payment system into Giving via a registered payment source.

- **Human URL:** [https://developer.planning.center/docs/#/apps/giving](https://developer.planning.center/docs/#/apps/giving)
- **Base URL:** `https://api.planningcenteronline.com/giving/v2`

#### Tags

- Giving
- Donations
- Funds
- Payments

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/giving)
- [Documentation](https://github.com/planningcenter/developers/blob/main/guides/giving_donations_integration.md)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Groups API

Manage small groups - group types, individual groups, their memberships and members, group events and attendance, tags, and enrollment. Read the group directory and write membership changes.

- **Human URL:** [https://developer.planning.center/docs/#/apps/groups](https://developer.planning.center/docs/#/apps/groups)
- **Base URL:** `https://api.planningcenteronline.com/groups/v2`

#### Tags

- Groups
- Small Groups
- Memberships
- Events

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/groups)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Check-Ins API

Read attendance and check-in data - check-ins, events and their event times, locations, stations, and the people checked in. Track headcounts and secure child check-in across events.

- **Human URL:** [https://developer.planning.center/docs/#/apps/check-ins](https://developer.planning.center/docs/#/apps/check-ins)
- **Base URL:** `https://api.planningcenteronline.com/check-ins/v2`

#### Tags

- Check-Ins
- Attendance
- Events
- Security

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/check-ins)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Calendar API

Manage church calendaring and facility scheduling - events and their event instances, room and equipment resources, resource requests, conflicts, and tags. Read the public event feed and manage room bookings.

- **Human URL:** [https://developer.planning.center/docs/#/apps/calendar](https://developer.planning.center/docs/#/apps/calendar)
- **Base URL:** `https://api.planningcenteronline.com/calendar/v2`

#### Tags

- Calendar
- Events
- Resources
- Scheduling

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/calendar)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Registrations API

Read event signups and registration data - signups (events), their categories and campuses, attendees, selection types, and emergency contacts. Surface live availability, times, and descriptions for public event listings.

- **Human URL:** [https://developer.planning.center/docs/#/apps/registrations](https://developer.planning.center/docs/#/apps/registrations)
- **Base URL:** `https://api.planningcenteronline.com/registrations/v2`

#### Tags

- Registrations
- Signups
- Events
- Payments

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/registrations)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Publishing API

Read-only access to published sermon content - channels, series, episodes and their episode times, speakers, and speakerships. Syndicate sermon media into external sites, apps, and podcast feeds.

- **Human URL:** [https://developer.planning.center/docs/#/apps/publishing](https://developer.planning.center/docs/#/apps/publishing)
- **Base URL:** `https://api.planningcenteronline.com/publishing/v2`

#### Tags

- Publishing
- Sermons
- Media
- Podcasting

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/publishing)
- [Documentation](https://www.planningcenter.com/changelog/publishing/25080772906139-new-publishing-sermons-api)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planning Center Webhooks API

Subscribe to create, update, and destroy events across the Planning Center products. Manage webhook subscriptions, browse the catalog of available events, and inspect deliveries and their event payloads. Delivery is outbound HTTPS POST to your endpoint - there is no public WebSocket surface.

- **Human URL:** [https://developer.planning.center/docs/#/apps/webhooks](https://developer.planning.center/docs/#/apps/webhooks)
- **Base URL:** `https://api.planningcenteronline.com/webhooks/v2`

#### Tags

- Webhooks
- Events
- Notifications
- Integration

#### Properties

- [API Reference](https://developer.planning.center/docs/#/apps/webhooks)
- [Documentation](https://www.planningcenter.com/blog/2017/09/webhooks)
- [OpenAPI](openapi/planning-center-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/planning-center.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planning-center.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/planningcenter)
- [LinkedIn](https://www.linkedin.com/company/planning-center)
- [Website](https://www.planningcenter.com)
- [Documentation](https://developer.planning.center/docs/)
- [Plans](plans/planning-center-plans-pricing.yml)
- [Rate Limits](rate-limits/planning-center-rate-limits.yml)
- [Fin Ops](finops/planning-center-finops.yml)

## Authentication

- **Personal Access Token** — HTTP Basic auth with an application id (username) and secret (password), for single-account scripts.
- **OAuth 2.0** — authorization code flow (PKCE recommended, OpenID Connect supported) for multi-organization apps. Authorize at `https://api.planningcenteronline.com/oauth/authorize`, token at `https://api.planningcenteronline.com/oauth/token`. Per-product scopes: `people`, `services`, `giving`, `groups`, `check_ins`, `calendar`, `registrations`, `publishing`.

All requests require a `User-Agent` header. Responses conform to the JSON:API 1.0 specification.

## Rate Limits

Default 100 requests per 20 seconds per authenticated user (75 per 20 seconds for requests with an offset above 30,000). Exceeding the limit returns HTTP 429 with a `Retry-After` header; every response carries `X-PCO-API-Request-Rate-Limit`, `X-PCO-API-Request-Rate-Period`, and `X-PCO-API-Request-Rate-Count`.

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
