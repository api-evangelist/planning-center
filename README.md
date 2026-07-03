# Planning Center (planning-center)

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
