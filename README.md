# MCP Personal Assistant

AI assistant and reusable MCP servers for Gmail and Google Calendar, with additional examples of external tools and local-model integration.

> Portfolio-ready, sanitized n8n workflows. Credentials and personal/course-specific data are intentionally excluded.

## Workflows

- `personal-ai-assistant.json` — Asistente personal
- `gmail-mcp-server.json` — Gmail MCP - Server
- `calendar-mcp-server.json` — MCP Google Calendar - Server
- `pokemon-tool-example.json` — Pokemon finder Tool
- `wikipedia-agent-example.json` — Wikipedia - Agente

## Architecture

The repository separates orchestration from credentials and external service configuration. n8n coordinates triggers, validation, integrations, AI/tool execution and persistence while external systems remain independently replaceable.

## Getting started

1. Run or connect to an n8n instance.
2. Import the JSON files from `workflows/`.
3. Create the required credentials inside n8n and bind them to the imported nodes.
4. Replace every `REPLACE_WITH_*` placeholder.
5. Execute with test data before activating schedules or public webhooks.

## Security

The workflows in this repository are sanitized portfolio versions. Credential bindings, pinned execution data, personal emails, account identifiers and embedded API keys were removed or replaced with placeholders.

Before importing:

1. Create credentials directly in n8n.
2. Rebind each credential-dependent node.
3. Replace `REPLACE_WITH_*` placeholders with your own resources.
4. Do not commit `.env` or exported credentials.
5. Validate webhook authentication, authorization and rate limits before exposing any endpoint publicly.

## Portfolio context

This repository refactors training workflows into a clean engineering showcase. It is intended to demonstrate orchestration, integrations, AI automation and production-minded patterns rather than publish third-party credentials or course-specific account data.

## License

MIT. Review the terms of every external API/service before production use.
