# Percolate plugins

The Percolate plugin connects Claude, Codex and ChatGPT to [Percolate](https://www.percolationlabs.ai), so your AI can research with you, save private drafts that show where each claim comes from, and revise them. You sign in to Percolate and allow the app the first time it uses a tool. Nothing you save is public until you publish it.

## Install

### Claude Desktop

1. Open **Customize → Plugins**.
2. Choose **Add marketplace** and enter `Percolation-Labs/percolate-plugins`.
3. Install **Percolate**. Sign in to Percolate and choose **Allow** when asked.

### Claude Code

```
/plugin marketplace add Percolation-Labs/percolate-plugins
/plugin install percolate@percolation-labs
```

Run `/mcp` to sign in to Percolate.

### Codex

```
codex plugin marketplace add Percolation-Labs/percolate-plugins
codex plugin add percolate@percolation-labs
```

Codex asks you to sign in to Percolate the first time a tool runs.

### ChatGPT, and Claude on the web or your phone

Add Percolate as a connector with the address `https://www.percolationlabs.ai/mcp`. [Connect your AI](https://www.percolationlabs.ai/app/connections) walks through it for each app.

## What's here

| Path | For |
|---|---|
| `plugins/percolate/` | The plugin: both manifests, the MCP connection and four skills. |
| `.claude-plugin/marketplace.json` | The marketplace Claude reads. |
| `.agents/plugins/marketplace.json` | The marketplace Codex and ChatGPT read. |

## Links

[Privacy](https://www.percolationlabs.ai/privacy.html) · [Terms](https://www.percolationlabs.ai/terms.html) · [Support](https://www.percolationlabs.ai/support.html)
