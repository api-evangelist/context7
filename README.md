# Context7 (context7)

Context7 is an Upstash service providing up-to-date, version-specific documentation and code examples for libraries and frameworks, exposed as both a REST API and a Model Context Protocol (MCP) server so AI coding assistants can fetch authoritative reference material at prompt time.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/context7/refs/heads/main/apis.yml)

## Scope

- **Type:** Contract
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags:

 - AI, Context, Documentation, LLM, MCP

## Timestamps

- **Created:** 2026-03-16
- **Modified:** 2026-04-28

## APIs

### Context7 REST API
The Context7 REST API exposes endpoints for searching libraries, retrieving documentation context for LLMs, refreshing indexed sources, and submitting new sources (GitHub repositories, OpenAPI specs, llms.txt files, websites, and Confluence spaces). Endpoints span v1 and v2 paths under https://context7.com/api and use Bearer token authentication with keys issued from the Context7 dashboard.

**Human URL:** [https://context7.com/docs/api-guide](https://context7.com/docs/api-guide)

#### Tags:

 - Documentation, LLM, REST, Search

#### Properties

- [Documentation](https://context7.com/docs/api-guide)
- [LLMsTxt](https://context7.com/docs/llms.txt)

### Context7 MCP Server
The Context7 MCP Server implements the Model Context Protocol so AI coding assistants such as Cursor, Claude, and Windsurf can call Context7 tools directly from a developer's editor. It exposes resolve-library-id (mapping a library name to a Context7-compatible identifier) and query-docs (returning documentation snippets for a given library and query) and is hosted at https://mcp.context7.com/mcp with API key authentication.

**Human URL:** [https://github.com/upstash/context7](https://github.com/upstash/context7)

#### Tags:

 - AI, Context, LLM, MCP

#### Properties

- [Documentation](https://github.com/upstash/context7)
- [GitHubRepository](https://github.com/upstash/context7)

### Context7 CLI
The Context7 CLI (ctx7) is a command-line tool for querying the Context7 index from the terminal. It provides ctx7 library for searching the catalog by library name and ctx7 docs for retrieving documentation using a Context7-compatible library ID, useful for scripting and local developer workflows.

**Human URL:** [https://github.com/upstash/context7](https://github.com/upstash/context7)

#### Tags:

 - CLI, Documentation, Tooling

#### Properties

- [Documentation](https://github.com/upstash/context7)
- [GitHubRepository](https://github.com/upstash/context7)

## Common Properties

- [Website](https://context7.com/)
- [Documentation](https://context7.com/docs)
- [Dashboard](https://context7.com/dashboard)
- [GitHub Organization](https://github.com/upstash)
- [GitHubRepository](https://github.com/upstash/context7)
- [Pricing](https://context7.com/pricing)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
