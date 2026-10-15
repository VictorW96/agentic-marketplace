# Agentic Marketplace

A [Claude plugin marketplace](https://code.claude.com/docs/en/plugins/create-marketplace) with plugins for Claude Cowork, Claude Desktop and Claude Code.

## Add this marketplace

- **Claude Cowork / Desktop:** *Customize → Plugins → Add marketplace* → `VictorW96/agentic-marketplace`
- **Claude Code:**
  ```
  /plugin marketplace add VictorW96/agentic-marketplace
  ```

## Plugins

| Plugin | Description | Source |
|---|---|---|
| [`windows-server-search`](plugins/windows-server-search) | Searches Windows file servers through their Windows Search index. Works automatically with the network drives already mapped on the PC. Windows only. | [windows-server-search-mcp](https://github.com/VictorW96/windows-server-search-mcp) |

Install it with `/plugin install windows-server-search@agentic-marketplace`, or from the Plugins page in Cowork.

## Publishing

Release tooling builds the plugins in their source repositories and copies them here. For example, `scripts/release.sh` in
windows-server-search-mcp builds the plugin, copies it to `plugins/<name>/` and updates `.claude-plugin/marketplace.json`.
Don't edit the files under `plugins/` by hand.
