# WeMetOnce AI Integrations

Integration and distribution metadata for **WeMetOnce**, a service that helps people find and reconnect with someone from their past.

## What this repository contains

This repository contains only public integration metadata, documentation, and configuration for AI platforms and MCP ecosystems.

It does **not** contain the WeMetOnce application source code, database, user accounts, private messages, credentials, admin data, or moderation data.

## MCP endpoint

The integrations connect to the production WeMetOnce MCP endpoint:

`https://www.wemetonce.com/api/mcp`

The MCP service is read-only and exposes only approved public Lost Connection posts.

Available tools:

- `search_lost_connections` — search approved public Lost Connection posts.
- `get_lost_connection` — retrieve one approved public Lost Connection post by ID.

## Privacy boundary

AI integrations do not provide access to:

- private accounts
- private messages
- credentials or authentication secrets
- admin or moderation data
- unapproved or private Lost Connection posts

Users and AI platforms remain subject to their own terms and privacy policies.

## Integration model

```text
AI platform / MCP ecosystem
          |
          v
This public integration repository
          |
          v
https://www.wemetonce.com/api/mcp
          |
          v
WeMetOnce production application
```

The integration layer is intentionally separated from the main WeMetOnce application repository.

## Links

- Website: https://www.wemetonce.com/
- Privacy: https://www.wemetonce.com/privacy
- Terms: https://www.wemetonce.com/terms
- Support: https://www.wemetonce.com/customer-support
- Main application repository: https://github.com/devworksarav/wemetonce
