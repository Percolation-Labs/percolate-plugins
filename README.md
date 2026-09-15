# Percolate plugins

The Percolate plugin connects your AI to [Percolate](https://www.percolationlabs.ai), so it can research with you, save private drafts that show where each claim comes from, and revise them. Nothing you save is public until you publish it.

## What has been tested

| | Status |
|---|---|
| Claude Code: add this marketplace and install the plugin from GitHub | Tested on 15 September 2026 |
| Codex: add this marketplace and install the plugin from GitHub | Tested on 15 September 2026 |
| Claude on the web or desktop: installing through **Customize → Plugins** | Not yet tested. The menu exists; the install has not been run |
| Signing in to Percolate through the plugin, in any app | Not yet tested |
| ChatGPT | Not available as a plugin. ChatGPT installs plugins from its own directory, and Percolate is not listed. Use a connector instead (below) |

## Install

### Claude on the web or desktop (not yet tested)

1. Open **Customize → Plugins**.
2. Choose **Add → Add marketplace** and enter `Percolation-Labs/percolate-plugins`.
3. Install **Percolate**. If Claude asks you to connect, sign in to Percolate and choose **Allow**.

### Claude Code

```
/plugin marketplace add Percolation-Labs/percolate-plugins
/plugin install percolate@percolation-labs
```

Then run `/mcp` to connect Percolate. Signing in this way has not been tested yet.

### Codex

```
codex plugin marketplace add Percolation-Labs/percolate-plugins
codex plugin add percolate@percolation-labs
```

Signing in to Percolate from Codex has not been tested yet.

### ChatGPT, and any app without plugins

Add Percolate as a connector with the address `https://www.percolationlabs.ai/mcp`. [Connect your AI](https://www.percolationlabs.ai/app/connections) walks through it for each app.

## What's here

| Path | For |
|---|---|
| `plugins/percolate/` | The plugin: both manifests, the MCP connection and four skills. |
| `.claude-plugin/marketplace.json` | The marketplace Claude reads. |
| `.agents/plugins/marketplace.json` | The marketplace in the Agent Plugins format, which Codex reads. |

## Links

[Privacy](https://www.percolationlabs.ai/privacy.html) · [Terms](https://www.percolationlabs.ai/terms.html) · [Support](https://www.percolationlabs.ai/support.html)
