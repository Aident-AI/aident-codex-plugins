---
name: aident
description: Use Aident Loadout from Codex to discover Apps and Actions, read Skills, check connected accounts in Vault, execute authorized tasks, and review action calls in Audit through the Aident MCP server.
---

# Aident Loadout

Use this skill when the user asks Codex to use Aident Loadout capabilities, connect an App, execute an Action, or inspect Audit history.

## Workflow

1. Prefer the plugin's `aident` MCP server for live Loadout data and Actions.
2. Start with capability search when the user describes a task. Use the exact capability names returned by discovery.
3. Read the selected capability's live input schema and check its required integrations in Vault before execution.
4. If an integration is missing, use the returned Loadout connection flow and tell the user which account or service needs authorization. Never request raw credentials in chat.
5. Execute within the user's authorized scope and honor the capability's approval requirements. An Action executes an app operation; a Skill supplies authored instructions.
6. Verify the result and use Audit history to recover uncertain execution outcomes before retrying an action that may already have happened.

## Common requests

- Find a Loadout tool for a task.
- Discover and execute an authorized Action.
- Find and read a Skill.
- Check connected Apps in Vault.
- Connect a missing integration.
- Review recent Loadout action calls in Audit.

## Authentication

The plugin supplies `https://loadout.aident.ai/mcp`. Authenticate through the MCP OAuth flow when prompted. Do not ask for raw Aident access tokens or manually edit Codex MCP configuration when this plugin is installed.
