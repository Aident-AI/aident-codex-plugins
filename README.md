# Aident Codex Plugins

This repository publishes the Aident plugin marketplace for Codex.

## Install

```bash
codex plugin marketplace add Aident-AI/aident-codex-plugins
```

Then open the Codex plugin directory, install **Aident**, and authenticate when prompted.

## What It Adds

- Aident MCP server: `https://loadout.aident.ai/mcp`
- Loadout guidance for discovering Apps, Actions and Skills, connecting accounts through Vault, and reviewing Audit
- Plugin metadata and assets for the Codex plugin directory

## Development

Plugin files live under `plugins/aident/`.

```text
.agents/plugins/marketplace.json
plugins/aident/.codex-plugin/plugin.json
plugins/aident/.mcp.json
plugins/aident/skills/aident/SKILL.md
plugins/aident/assets/
```

To test a local checkout:

```bash
codex plugin marketplace add /path/to/aident-codex-plugins
```

To update an installed marketplace after changes:

```bash
codex plugin marketplace upgrade aident
```
