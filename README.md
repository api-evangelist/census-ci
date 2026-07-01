# Census (census-ci)

Census is a reverse ETL and data activation platform that syncs modeled data out of the cloud data warehouse into 200+ business tools (CRM, ads, marketing, support, and analytics), plus an Audience Hub for building and activating segments. The Census Management API (base `https://app.getcensus.com/api/v1`, Bearer workspace token) lets teams manage sources, destinations, syncs, sync runs, datasets/models, connections, and segments/audiences programmatically.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/census-ci/refs/heads/main/apis.yml)

## Tags

- Reverse ETL
- Data Activation
- Data Warehouse
- Syncs
- Audience Hub
- Data Marketing

## Timestamps

- **Created:** 2026-07-01
- **Modified:** 2026-07-01

## APIs

### Census Sources API

Manage source connections - the warehouses and databases (Snowflake, BigQuery, Redshift, Databricks, Postgres) Census reads modeled data from. List, fetch, and create sources, and enumerate their available source objects.

- **Human URL:** [https://developers.getcensus.com/api-reference/sources](https://developers.getcensus.com/api-reference/sources)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Sources
- Data Warehouse
- Connections

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/sources)
- [API Reference](https://developers.getcensus.com/api-reference/sources/list-sources)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Destinations API

Manage destination connections across 200+ supported business tools and inspect the object types and fields Census can write to per connector service.

- **Human URL:** [https://developers.getcensus.com/api-reference/destinations](https://developers.getcensus.com/api-reference/destinations)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Destinations
- Connectors
- Business Tools

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/destinations)
- [API Reference](https://developers.getcensus.com/api-reference/connectors/list-destination-object-types)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Syncs API

List, fetch, create, update, delete, and trigger syncs. A sync maps a source dataset/model to a destination object with field mappings, an operation (upsert, mirror, append, update), and a schedule. The trigger endpoint powers Airflow, Dagster, Prefect, and dbt Cloud orchestration.

- **Human URL:** [https://developers.getcensus.com/api-reference/syncs](https://developers.getcensus.com/api-reference/syncs)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Syncs
- Reverse ETL
- Mappings

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/syncs/list-syncs)
- [API Reference](https://developers.getcensus.com/api-reference/syncs/list-syncs)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Sync Runs API

Read the execution history and live status of syncs - records processed, updated, failed, and invalid per run - to monitor and observe data activation pipelines.

- **Human URL:** [https://developers.getcensus.com/api-reference/sync-runs](https://developers.getcensus.com/api-reference/sync-runs)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Sync Runs
- Observability
- Status

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/sync-runs)
- [API Reference](https://developers.getcensus.com/api-reference/sync-runs/list-sync-runs)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Datasets & Models API

Manage the SQL models and datasets that define the source-of-truth data Census syncs - list, fetch, create, and update SQL-backed models and datasets used as sync sources.

- **Human URL:** [https://developers.getcensus.com/api-reference/models](https://developers.getcensus.com/api-reference/models)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Datasets
- Models
- SQL

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/models)
- [API Reference](https://developers.getcensus.com/dataset-api/guide)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Connections API

List available connectors and, for a given destination service, enumerate its supported object types so integrations can discover what Census can read from and write to.

- **Human URL:** [https://developers.getcensus.com/api-reference/connectors](https://developers.getcensus.com/api-reference/connectors)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Connections
- Connectors
- Catalog

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/connectors)
- [API Reference](https://developers.getcensus.com/api-reference/connectors/list-destination-object-types)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Census Segments & Audiences API

Build and activate audience segments in the Census Audience Hub - list, fetch, and create segments defined over an entity, then sync those audiences to marketing and advertising destinations.

- **Human URL:** [https://developers.getcensus.com/api-reference/segments](https://developers.getcensus.com/api-reference/segments)
- **Base URL:** `https://app.getcensus.com/api/v1`

#### Tags

- Segments
- Audiences
- Audience Hub

#### Properties

- [Documentation](https://developers.getcensus.com/api-reference/segments)
- [API Reference](https://developers.getcensus.com/api-reference/segments/list-segments)
- [OpenAPI](openapi/census-ci-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/census-ci.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/census-ci.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [GitHub Organization](https://github.com/sutrolabs)
- [LinkedIn](https://www.linkedin.com/company/getcensus)
- [Website](https://www.getcensus.com)
- [Documentation](https://developers.getcensus.com)
- [Plans](plans/census-ci-plans-pricing.yml)
- [Rate Limits](rate-limits/census-ci-rate-limits.yml)
- [Fin Ops](finops/census-ci-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com

---

> Note: Census was acquired by Fivetran. The `developers.getcensus.com` and `docs.getcensus.com` documentation now 301-redirects to `fivetran.com/docs/activations`, but the Census Management API and its `https://app.getcensus.com/api/v1` base URL remain the operative surface.
