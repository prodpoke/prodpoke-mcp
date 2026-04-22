# Changelog

All notable changes to the ProdPoke MCP Server are documented here.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] — 2026-04-22

### Added
- Initial public release of the hosted ProdPoke MCP server at `https://prodpoke.com/v1/mcp`.
- `chat(message, session_id?)` — stateful conversational QA tool. Scans URLs, runs user-flow
  tests, investigates prior findings, and carries context across turns via `session_id`.
- `get_credit_balance()` — returns the current credit balance for the authenticated account.
- Bearer-token authentication via `Authorization: Bearer pp_...`. Keys are created at
  [/app/settings/keys](https://prodpoke.com/app/settings/keys).
- Streamable HTTP transport (MCP spec 2025-11-05); no local install required.
