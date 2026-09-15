# Percolate plugins

The Percolate plugin connects your AI to [Percolate](https://www.percolationlabs.ai), so it can research with you, save private drafts that show where each claim comes from, and revise them. Nothing you save is public until you publish it.

## What has been tested

| | Status |
|---|---|
| Claude on the web: add this marketplace and add the plugin | Tested on 15 September 2026. The plugin's connector was already connected on that account, so connecting for the first time from the plugin has not been tested |
| Claude Code: install from GitHub, then sign in to Percolate | Tested on 15 September 2026: signed in, and the connection checked as connected |
| Codex: install from GitHub, then sign in to Percolate | Tested on 15 September 2026: signed in. The account had already allowed Codex, so the Allow page was not shown |
| ChatGPT desktop app: **Plugins → Add → Add a marketplace** | Not yet tested. The app offers it (ChatGPT 26.903) |
| ChatGPT on the web or a phone | Not known whether a plugin added in the desktop app works there. Use a connector (below) |

## Install

### Claude on the web or desktop

1. Open **Customize → Plugins**.
2. Choose **Add → Add marketplace → Add from a repository**. Search for or paste `Percolation-Labs/percolate-plugins`, and choose **Sync**.
3. Choose **Add** on **Percolate**. If its connector is not connected, connect it: sign in to Percolate and choose **Allow**.

### Claude Code

```
/plugin marketplace add Percolation-Labs/percolate-plugins
/plugin install percolate@percolation-labs
```

Then run `/mcp`, or `claude mcp login plugin:percolate:percolate`, to sign in to Percolate.

### Codex

```
codex plugin marketplace add Percolation-Labs/percolate-plugins
codex plugin add percolate@percolation-labs
codex mcp login percolate
```

### ChatGPT desktop app (not yet tested)

1. Open **Plugins**.
2. Choose **Add → Add a marketplace**, and enter `Percolation-Labs/percolate-plugins` as the **Source**.
3. Install **Percolate**. If ChatGPT asks you to connect, sign in to Percolate and choose **Allow**.

### ChatGPT on the web or a phone, and any app without plugins

Add Percolate as a connector with the address `https://www.percolationlabs.ai/mcp`. [Connect your AI](https://www.percolationlabs.ai/app/connections) walks through it for each app.

## What's here

| Path | For |
|---|---|
| `plugins/percolate/` | The plugin: both manifests, the MCP connection and four skills. |
| `.claude-plugin/marketplace.json` | The marketplace Claude reads. |
| `.agents/plugins/marketplace.json` | The marketplace in the Agent Plugins format. Codex reads it (tested); the ChatGPT desktop app can add it (not yet tested). |

## License

[Apache-2.0](LICENSE). The skills here are the starting points; the guides they fetch are served by Percolate to signed-in writers and are not part of this repository.

## Links

[Privacy](https://www.percolationlabs.ai/privacy.html) · [Terms](https://www.percolationlabs.ai/terms.html) · [Support](https://www.percolationlabs.ai/support.html)
