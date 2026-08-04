# Planet Labs (planet-labs)

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

Planet Labs operates the world's largest commercial Earth observation constellation, imaging the entire landmass of the planet daily with its PlanetScope satellites and capturing high-resolution targeted imagery with SkySat and Pelican. The Planet Insights Platform is API-first: developers search the archive through the Data and Catalog APIs, order processed bundles through the Orders API, set up standing area-of-interest deliveries through the Subscriptions API, request tip-and-cue collections through the Tasking API, and consume mosaics through the Basemaps and Tiles APIs. Analytics, Processing, Statistical, and Batch APIs run server-side workflows over the catalog and over Planetary Variables. All APIs sit under api.planet.com, authenticate with an API key over HTTP Basic, and are wrapped by the official Planet Python SDK.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/planet-labs/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/planet-labs/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Earth Observation
- Satellite Imagery
- Geospatial
- PlanetScope
- SkySat
- Pelican
- Tasking
- Basemaps
- Analytics
- Subscriptions
- STAC
- GIS

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

### Planet Data API

Programmatic search over Planet's imagery catalog by AOI, time window, cloud cover, item type, and asset type. Returns item and asset metadata for downstream activation and download.

- **Human URL:** [https://docs.planet.com/develop/apis/data/](https://docs.planet.com/develop/apis/data/)
- **Base URL:** `https://api.planet.com/data/v1`

#### Tags

- Search
- Catalog
- Imagery

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/data/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Catalog API

STAC-based search and access layer over Planet imagery metadata, providing a standards-aligned interface to the archive.

- **Human URL:** [https://docs.planet.com/develop/apis/](https://docs.planet.com/develop/apis/)
- **Base URL:** `https://api.planet.com`

#### Tags

- STAC
- Catalog
- Metadata

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Orders API

Request preparation and delivery of imagery bundles with optional processing operations (clip, composite, harmonize, reproject, band math, file format), and deliver to cloud destinations (S3, GCS, Azure) or direct download URLs.

- **Human URL:** [https://docs.planet.com/develop/apis/orders/](https://docs.planet.com/develop/apis/orders/)
- **Base URL:** `https://api.planet.com/compute/ops`

#### Tags

- Orders
- Delivery
- Processing

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/orders/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Subscriptions API

Standing subscriptions that deliver new imagery and analytic feeds to a cloud destination automatically as new acquisitions clear the AOI and cloud-cover filter.

- **Human URL:** [https://docs.planet.com/develop/apis/subscriptions/](https://docs.planet.com/develop/apis/subscriptions/)
- **Base URL:** `https://api.planet.com/subscriptions/v1`

#### Tags

- Subscriptions
- Streaming
- Cloud Delivery

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/subscriptions/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Basemaps API

Discover, view, and download Planet's PlanetScope monitoring and visual basemap mosaics covering the global landmass at regular cadence.

- **Human URL:** [https://docs.planet.com/develop/apis/basemaps/](https://docs.planet.com/develop/apis/basemaps/)
- **Base URL:** `https://api.planet.com/basemaps/v1`

#### Tags

- Basemaps
- Mosaics
- Imagery

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/basemaps/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Tasking API

Tasking interface for SkySat and Pelican constellations. Submit collection requests against a target geometry and time window and track capture and delivery status.

- **Human URL:** [https://docs.planet.com/develop/apis/tasking/](https://docs.planet.com/develop/apis/tasking/)
- **Base URL:** `https://api.planet.com/tasking/v2`

#### Tags

- Tasking
- SkySat
- Pelican
- Tip and Cue

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/tasking/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Analytics API

Access to Planet Analytics Feeds, including building, road, ship, and change detection outputs derived from the imagery archive.

- **Human URL:** [https://docs.planet.com/develop/apis/analytics/](https://docs.planet.com/develop/apis/analytics/)
- **Base URL:** `https://api.planet.com/analytics`

#### Tags

- Analytics
- Detection
- Change
- ML

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/analytics/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Processing API

Run custom processing scripts on raw bands and derive indices (NDVI, EVI, etc.) over Planet imagery without downloading source data.

- **Human URL:** [https://docs.planet.com/develop/apis/](https://docs.planet.com/develop/apis/)
- **Base URL:** `https://api.planet.com`

#### Tags

- Processing
- Indices
- NDVI

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Statistical API

Compute per-AOI statistics (mean, median, percentiles, histograms) over imagery and analytic layers without requiring full raster downloads.

- **Human URL:** [https://docs.planet.com/develop/apis/](https://docs.planet.com/develop/apis/)
- **Base URL:** `https://api.planet.com`

#### Tags

- Statistics
- Zonal Stats
- Analytics

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Tiles API

XYZ and WMTS tile services for visualizing PlanetScope and SkySat scenes and basemaps in web mapping clients.

- **Human URL:** [https://docs.planet.com/develop/apis/](https://docs.planet.com/develop/apis/)
- **Base URL:** `https://tiles.planet.com`

#### Tags

- Tiles
- XYZ
- WMTS
- Visualization

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Features API

Save and manage Areas of Interest (features and feature collections) for reuse across Subscriptions, Orders, and Tasking.

- **Human URL:** [https://docs.planet.com/develop/apis/](https://docs.planet.com/develop/apis/)
- **Base URL:** `https://api.planet.com/features/v1`

#### Tags

- Features
- AOI
- GeoJSON

#### Properties

- [Documentation](https://docs.planet.com/develop/apis/)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Planet Python SDK

Official Python SDK (planet on PyPI) and CLI for working with all Planet APIs, including async clients for search, orders, subscriptions, and data activation.

- **Human URL:** [https://github.com/planetlabs/planet-client-python](https://github.com/planetlabs/planet-client-python)
- **Base URL:** `https://github.com/planetlabs/planet-client-python`

#### Tags

- SDK
- Python
- CLI

#### Properties

- [Repository](https://github.com/planetlabs/planet-client-python)
- [Postman Collection](collections/planet-labs.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/planet-labs.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://www.planet.com/)
- [Developers](https://www.planet.com/markets/developers/)
- [Documentation](https://docs.planet.com/)
- [API Reference](https://docs.planet.com/develop/apis/)
- [Insights Platform](https://www.planet.com/products/planet-insights-platform/)
- [GitHub Organization](https://github.com/planetlabs)
- [Blog](https://www.planet.com/pulse/)
- [Pricing](https://www.planet.com/pricing/)
- [Status](https://status.planet.com/)
- [LinkedIn](https://www.linkedin.com/company/planet-labs/)
- [X (Twitter)](https://x.com/planet)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
