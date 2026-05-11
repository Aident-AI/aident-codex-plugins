---
name: aident
description: Use Aident from Codex for capability discovery, skill execution, integration connection status, playbook generation and execution, templates, dashboards, and execution details through the Aident MCP server.
---

# Aident

Use this skill when the user asks Codex to work with Aident capabilities, integrations, playbooks, templates, dashboards, or execution history.

## Workflow

1. Prefer the `aident` MCP server tools for live Aident data and actions.
2. Start with capability search when the user asks for a task but does not know the exact skill or integration.
3. Check integration status before executing skills that require connected third-party accounts.
4. If an integration is missing, use the Aident integration connection flow and tell the user which account or service they need to authorize.
5. For playbook requests, generate or inspect the playbook first, then execute only after the user confirms externally visible actions.

## Common Requests

- Search for available Aident skills or integrations.
- Execute an Aident skill with user-provided inputs.
- Generate, list, inspect, update, or execute Aident playbooks.
- Search, inspect, or instantiate Aident templates.
- Check active playbooks, execution details, or execution messages.
- Connect missing integrations needed for a task.

## Notes

- Aident authentication is handled by the MCP OAuth flow at `https://app.aident.ai/api/mcp`.
- Do not ask the user for raw Aident access tokens.
- Do not manually edit Codex MCP config when this plugin is installed; the plugin supplies the MCP server configuration.
