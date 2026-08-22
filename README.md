# Context7 (context7)

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

Context7 is an Upstash service providing up-to-date, version-specific documentation and code examples for libraries and frameworks, exposed as both a REST API and a Model Context Protocol (MCP) server so AI coding assistants can fetch authoritative reference material at prompt time.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- AI
- Context
- Documentation
- LLM
- MCP

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-05-19

## APIs

### Context7 REST API

The Context7 REST API exposes endpoints for searching libraries, retrieving documentation context for LLMs, refreshing indexed sources, and submitting new sources (GitHub repositories, OpenAPI specs, llms.txt files, websites, and Confluence spaces). Endpoints span v1 and v2 paths under https://context7.com/api and use Bearer token authentication with keys issued from the Context7 dashboard.

- **Human URL:** [https://context7.com/docs/api-guide](https://context7.com/docs/api-guide)
- **Base URL:** `https://context7.com/api`

#### Tags

- Documentation
- LLM
- REST
- Search

#### Properties

- [Documentation](https://context7.com/docs/api-guide)
- [L L Ms Txt](https://context7.com/docs/llms.txt)
- [OpenAPI](openapi/context7-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/context7.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/context7.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Context7 MCP Server

The Context7 MCP Server implements the Model Context Protocol so AI coding assistants such as Cursor, Claude, and Windsurf can call Context7 tools directly from a developer's editor. It exposes resolve-library-id (mapping a library name to a Context7-compatible identifier) and query-docs (returning documentation snippets for a given library and query) and is hosted at https://mcp.context7.com/mcp with API key authentication.

- **Human URL:** [https://github.com/upstash/context7](https://github.com/upstash/context7)
- **Base URL:** `https://mcp.context7.com/mcp`

#### Tags

- AI
- Context
- LLM
- MCP

#### Properties

- [Documentation](https://github.com/upstash/context7)
- [GitHub Repository](https://github.com/upstash/context7)
- [Postman Collection](collections/context7.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/context7.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### Context7 CLI

The Context7 CLI (ctx7) is a command-line tool for querying the Context7 index from the terminal. It provides ctx7 library for searching the catalog by library name and ctx7 docs for retrieving documentation using a Context7-compatible library ID, useful for scripting and local developer workflows.

- **Human URL:** [https://github.com/upstash/context7](https://github.com/upstash/context7)

#### Tags

- CLI
- Documentation
- Tooling

#### Properties

- [Documentation](https://github.com/upstash/context7)
- [GitHub Repository](https://github.com/upstash/context7)
- [Postman Collection](collections/context7.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/context7.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Website](https://context7.com/)
- [Documentation](https://context7.com/docs)
- [Dashboard](https://context7.com/dashboard)
- [GitHub Organization](https://github.com/upstash)
- [GitHub Repository](https://github.com/upstash/context7)
- [Pricing](https://context7.com/pricing)
- [Integrations](https://context7.com/integrations)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
