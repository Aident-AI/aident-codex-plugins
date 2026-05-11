# Aident Codex Plugins

This repository publishes the Aident plugin marketplace for Codex.

## Install

```bash
codex plugin marketplace add Aident-AI/aident-codex-plugins
```

Then open the Codex plugin directory, install **Aident**, and authenticate when prompted.

## What It Adds

- Aident MCP server: `https://app.aident.ai/api/mcp`
- Aident workflow guidance for capability search, skills, integrations, playbooks, templates, and execution history
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
