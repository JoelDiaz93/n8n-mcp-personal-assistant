# MCP Personal Assistant — Architecture

## Purpose

AI assistant and reusable MCP servers for Gmail and Google Calendar, with additional examples of external tools and local-model integration.

## Design principles

- Keep n8n focused on orchestration.
- Isolate external integrations behind explicit nodes/tools.
- Keep credentials outside exported workflows.
- Make mutations explicit and auditable.
- Prefer deterministic validation for authorization and business rules.
- Add retries, idempotency and observability before production use.
