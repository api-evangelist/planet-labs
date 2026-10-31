# Planet Labs

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

Planet Labs operates the world's largest commercial Earth observation constellation, imaging the entire landmass of the planet daily with its PlanetScope satellites and capturing high-resolution targeted imagery with SkySat and Pelican. The Planet Insights Platform is API-first: developers search the archive through the Data and Catalog APIs, order processed bundles through the Orders API, set up standing area-of-interest deliveries through the Subscriptions API, request tip-and-cue collections through the Tasking API, and consume mosaics through the Basemaps and Tiles APIs. Analytics, Processing, Statistical, and Batch APIs run server-side workflows over the catalog and over Planetary Variables. All APIs sit under api.planet.com, authenticate with an API key over HTTP Basic, and are wrapped by the official Planet Python SDK.

**Areas:** Earth Observation · Satellite Imagery · Geospatial · PlanetScope · SkySat · Pelican · Tasking · Basemaps · Analytics · Subscription · STAC · GIS

## Planet Labs on APIs.io

Everything profiled for Planet Labs is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/planet-labs/](https://apis.io/providers/planet-labs/)** — or go straight to one of the APIs or properties below.

### APIs (18)

- [Planet Data API](https://apis.io/apis/planet-labs/data/) — Programmatic search over Planet's imagery catalog by AOI, time window, cloud cover, item type, and asset type. Returns item and asset metadata for…
- [Planet Catalog API](https://apis.io/apis/planet-labs/catalog/) — STAC-based search and access layer over Planet imagery metadata, providing a standards-aligned interface to the archive.
- [Planet Orders API](https://apis.io/apis/planet-labs/orders/) — Request preparation and delivery of imagery bundles with optional processing operations (clip, composite, harmonize, reproject, band math, file format), and…
- [Planet Subscriptions API](https://apis.io/apis/planet-labs/subscriptions/) — Standing subscriptions that deliver new imagery and analytic feeds to a cloud destination automatically as new acquisitions clear the AOI and cloud-cover…
- [Planet Basemaps API](https://apis.io/apis/planet-labs/basemaps/) — Discover, view, and download Planet's PlanetScope monitoring and visual basemap mosaics covering the global landmass at regular cadence.
- [Planet Tasking API](https://apis.io/apis/planet-labs/tasking/) — Tasking interface for SkySat and Pelican constellations. Submit collection requests against a target geometry and time window and track capture and delivery…
- [Planet Analytics API](https://apis.io/apis/planet-labs/analytics/) — Access to Planet Analytics Feeds, including building, road, ship, and change detection outputs derived from the imagery archive.
- [Planet Processing API](https://apis.io/apis/planet-labs/processing/) — Run custom processing scripts on raw bands and derive indices (NDVI, EVI, etc.) over Planet imagery without downloading source data.
- [Planet Statistical API](https://apis.io/apis/planet-labs/statistical/) — Compute per-AOI statistics (mean, median, percentiles, histograms) over imagery and analytic layers without requiring full raster downloads.
- [Planet Tiles API](https://apis.io/apis/planet-labs/tiles/) — XYZ and WMTS tile services for visualizing PlanetScope and SkySat scenes and basemaps in web mapping clients.
- [Planet Features API](https://apis.io/apis/planet-labs/features/) — Save and manage Areas of Interest (features and feature collections) for reuse across Subscriptions, Orders, and Tasking.
- [Planet Python SDK](https://apis.io/apis/planet-labs/python-sdk/) — Official Python SDK (planet on PyPI) and CLI for working with all Planet APIs, including async clients for search, orders, subscriptions, and data activation.
- [Planet Labs Data - Item Types API](https://apis.io/apis/planet-labs/planet-labs-data-item-types-api/) — Item type and asset type metadata.
- [Planet Labs Data - Items API](https://apis.io/apis/planet-labs/planet-labs-data-items-api/) — Item and asset retrieval.
- [Planet Labs Data - Search API](https://apis.io/apis/planet-labs/planet-labs-data-search-api/) — Catalog search and saved searches.
- [Planet Labs Data - Stats API](https://apis.io/apis/planet-labs/planet-labs-data-stats-api/) — Search-driven statistics.
- [Planet Labs Orders API](https://apis.io/apis/planet-labs/planet-labs-orders-api/) — Bundle preparation and delivery jobs.
- [Planet Labs Subscriptions API](https://apis.io/apis/planet-labs/planet-labs-subscriptions-api/) — Standing area-of-interest delivery feeds.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### GraphQL (1)

GraphQL schemas.

- [Moved to /providers/planet-labs/](https://apis.io/graphqls/planet-labs/planet-labs-graphql/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Planet Labs Agentic Access](https://apis.io/agentic-access/planet-labs/planet-labs-agentic-access/)

#### Collections (7)

Postman and Open Collection request collections.

- [Planet Insights Platform API](https://apis.io/collections/planet-labs/open-planet-labs/)
- [Planet Insights Platform Data - Item Types API](https://apis.io/collections/planet-labs/open-planet-labs-data-item-types-api/)
- [Planet Insights Platform Data - Item Types Data - Items API](https://apis.io/collections/planet-labs/open-planet-labs-data-items-api/)
- [Planet Insights Platform Data - Item Types Data - Search API](https://apis.io/collections/planet-labs/open-planet-labs-data-search-api/)
- [Planet Insights Platform Data - Item Types Data - Stats API](https://apis.io/collections/planet-labs/open-planet-labs-data-stats-api/)
- [Planet Insights Platform Data - Item Types Orders API](https://apis.io/collections/planet-labs/open-planet-labs-orders-api/)
- [Planet Insights Platform Data - Item Types Subscriptions API](https://apis.io/collections/planet-labs/open-planet-labs-subscriptions-api/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Planet Labs Authentication](https://apis.io/security/planet-labs/planet-labs-authentication/)
- [Planet Labs Domain Security](https://apis.io/security/planet-labs/planet-labs-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Planet Labs Plans Pricing](https://apis.io/plans/planet-labs/planet-labs-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Planet Labs Rate Limits](https://apis.io/rate-limits/planet-labs/planet-labs-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Planet Labs Finops](https://apis.io/finops/planet-labs/planet-labs-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.planet.com/)
- [Documentation](https://docs.planet.com/)
- [API reference](https://docs.planet.com/develop/apis/)
- [Pricing](https://www.planet.com/pricing/)
- [Blog](https://www.planet.com/pulse/)
- [GitHub](https://github.com/planetlabs)

## API Evangelist rating

**Kin Score 31.5** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 66.1 |
| Contract quality | 46.8 |
| Contract governance | 0.0 |
| Operational transparency | 23.7 |
| Developer ergonomics | 31.0 |
| Access clarity | 15.8 |

**Agent readiness 19.6** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | — |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 11.8** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/planet-labs/](https://apis.io/providers/planet-labs/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Planet Labs: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/planet-labs/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
