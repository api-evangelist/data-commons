# Data Commons (data-commons)

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

Data Commons is an open knowledge graph initiative led by Google that aggregates and harmonizes the world's public data into a single graph, making global statistical data simple to explore, query, and integrate through REST, Python, BigQuery, web component, and MCP interfaces.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/data-commons/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/data-commons/refs/heads/main/apis.yml)

## Scope

- **Position:** Consumer
- **Access:** 3rd-Party

## Tags

- Data Commons
- Knowledge Graph
- Open Data
- Public Data
- Statistics

## Timestamps

- **Created:** 2026-01-02
- **Modified:** 2026-05-19

## APIs

### Data Commons REST API V2

HTTP REST interface for retrieving statistical observations, exploring the Data Commons knowledge graph, and resolving entities to Data Commons IDs (DCIDs). Returns structured JSON data covering variables, places, and observations.

- **Human URL:** [https://docs.datacommons.org/api/rest/v2/](https://docs.datacommons.org/api/rest/v2/)

#### Tags

- Knowledge Graph
- REST
- Statistics

#### Properties

- [Documentation](https://docs.datacommons.org/api/rest/v2/)
- [A P I  Keys](https://apikeys.datacommons.org)
- [Reference](https://docs.datacommons.org/api/)
- [OpenAPI](openapi/data-commons-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/data-commons.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/data-commons.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Data Commons Python Client

Official Python client library that wraps the Data Commons REST API with native Pandas DataFrame support for analytical workflows and notebook integration.

- **Human URL:** [https://docs.datacommons.org/api/python/v2/](https://docs.datacommons.org/api/python/v2/)

#### Tags

- Pandas
- Python
- SDK

#### Properties

- [Documentation](https://docs.datacommons.org/api/python/v2/)
- [Py P I](https://pypi.org/project/datacommons-client/)
- [Postman Collection](collections/data-commons.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/data-commons.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Data Commons Google Sheets

Custom Google Sheets functions that pull Data Commons statistical data directly into spreadsheets without requiring an API key.

- **Human URL:** [https://docs.datacommons.org/api/sheets/](https://docs.datacommons.org/api/sheets/)

#### Tags

- Google Sheets
- Spreadsheets

#### Properties

- [Documentation](https://docs.datacommons.org/api/sheets/)
- [Postman Collection](collections/data-commons.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/data-commons.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Data Commons Web Components

Drop-in JavaScript/HTML web components for embedding Data Commons charts, maps, rankings, and visualizations in any website.

- **Human URL:** [https://docs.datacommons.org/api/web_components/](https://docs.datacommons.org/api/web_components/)

#### Tags

- JavaScript
- Visualization
- Web Components

#### Properties

- [Documentation](https://docs.datacommons.org/api/web_components/)
- [Postman Collection](collections/data-commons.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/data-commons.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Data Commons BigQuery

SQL access to Data Commons through Google BigQuery enabling complex analytical queries and joins with private datasets.

- **Human URL:** [https://docs.datacommons.org/api/bigquery.html](https://docs.datacommons.org/api/bigquery.html)

#### Tags

- BigQuery
- SQL

#### Properties

- [Documentation](https://docs.datacommons.org/api/bigquery.html)
- [Postman Collection](collections/data-commons.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/data-commons.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Data Commons MCP Server

Model Context Protocol server that lets AI agents query Data Commons conversationally, surfacing variables, places, and observations through natural language tools.

- **Human URL:** [https://docs.datacommons.org/api/mcp/](https://docs.datacommons.org/api/mcp/)

#### Tags

- AI Agents
- MCP
- Natural Language

#### Properties

- [Documentation](https://docs.datacommons.org/api/mcp/)
- [A P I  Keys](https://apikeys.datacommons.org)
- [Postman Collection](collections/data-commons.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/data-commons.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://datacommons.org/)
- [Documentation](https://docs.datacommons.org/)
- [A P I  Documentation](https://docs.datacommons.org/api/)
- [A P I  Keys](https://apikeys.datacommons.org)
- [GitHub Organization](https://github.com/datacommonsorg)
- [Blog](https://blog.datacommons.org/)
- [Vocabulary](vocabulary/data-commons-vocabulary.yml)
- [JSON-LD](json-ld/data-commons-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [M C P Server](https://blog.datacommons.org/2025/10/02/announcing-the-data-commons-model-context-protocol-server/)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
