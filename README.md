# innRoad (innroad)

innRoad is a cloud-based hotel property management system (PMS) that bundles PMS, a direct booking engine, and a channel manager (OTA distribution to Expedia, Booking.com, Airbnb, and others) into one platform, built for independent hotels, boutique properties, and small hotel management companies. innRoad also offers 40+ pre-built partner connections - point-of-sale (Lightspeed, Oracle Hospitality, Squirrel, Positouch, Uniwell), door locks (RemoteLock, Saflok, ONITY), guest messaging (Akia), accounting (M3, Inn-Flow), and in-house payment processing (innRoad Payments) - that are toggled on inside the application.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/innroad/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/innroad/refs/heads/main/apis.yml)

## API Access Model (Important)

**innRoad does not publish a public, self-service developer API.** There is no developer portal, no public API reference, no OpenAPI definition, and no documented WebSocket or webhook API at the time of cataloging. This entry is intentionally a stub that documents the company and its access model honestly rather than fabricating an API surface.

How integration actually works:

- **Partner-gated, pre-built connections.** Every listed integration (OTAs/channel management, POS, door locks, guest messaging, accounting) is built and maintained by innRoad's own engineering team and simply enabled per property inside the app - there is no self-serve developer console or API key signup.
- **"API integration" is used loosely.** Support articles occasionally reference "innRoad's API integration" when describing how a specific partner connection (e.g., Akia guest messaging) syncs reservation and guest data, but no technical detail - endpoint paths, request/response schema, or base URL - is made public anywhere.
- **Independently confirmed as closed.** A 2026 third-party PMS API scorecard explicitly categorizes innRoad as "No public API," with self-serve access, authentication docs, AI-readiness, and an app marketplace all marked "No" or "n/a."

Because no public endpoints, request/response schemas, or authentication details are documented, no `openapi/`, `collections/`, `rate-limits/`, or `finops/` artifacts are included, and no `apis` array is asserted in `apis.yml`. If innRoad opens partner API documentation in the future, this entry can be expanded with real, sourced endpoints.

## Tags

- Hospitality
- Hotel PMS
- Property Management
- Booking Engine
- Channel Manager
- Revenue Management
- Independent Hotels
- Partner Integrations

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## Pricing

innRoad uses custom, property-based pricing rather than published self-serve tiers. Its own FAQ cites the core PMS as "typically around $150 per month for most properties," billed month-to-month with no long-term contract ("cancel anytime"), and a free trial/demo is available. Custom packages exist for hotel management companies needing volume discounts, multi-product discounts (Booking Engine, Channel Manager, Revenue Management, innRoad Payments), or country-specific training. See [Plans & Pricing](plans/innroad-plans-pricing.yml).

## Common Properties

- [LinkedIn](https://www.linkedin.com/company/innroad-inc)
- [Website](https://www.innroad.com/)
- [Plans](plans/innroad-plans-pricing.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
