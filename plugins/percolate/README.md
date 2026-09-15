# Percolate plugin

Connects your AI to [Percolate](https://www.percolationlabs.ai), where you save, read and revise research packages: arguments a reader can check, with the evidence behind each claim. Everything you save stays private until you publish it.

## What's in it

| File | What it does |
|---|---|
| `plugin.json` | The [Agent Plugins](https://agent-plugins.org) manifest, read by ChatGPT and Codex, with its listing details under `extensions.com.openai`. |
| `.claude-plugin/plugin.json` | The same plugin, described for Claude. |
| `mcp.json`, `.mcp.json` | The same content under both names: connects to Percolate at `https://www.percolationlabs.ai/mcp`. You sign in to Percolate the first time a tool runs, and no token is copied. |
| `skills/` | Four workflows: making a package, importing a story, finding counterpoints and checking a package. Each follows the matching guide Percolate's server provides. |
| `assets/logo.png` | Percolate's logo. |

Installation is in the [repository README](../../README.md).
