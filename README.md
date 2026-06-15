# Planet Labs (planet-labs)

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
