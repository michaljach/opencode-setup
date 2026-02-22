# OpenCode Setup Documentation

This repository is a documentation artifact for the current OpenCode environment on this machine.

It intentionally stores documentation only, not a raw file backup directory.

## Included Files

- `README.md` (this document)
- `AGENTS.md` (copied from global `~/.config/opencode/AGENTS.md`)

## Current OpenCode Snapshot

### Config location

- `~/.config/opencode/opencode.json`
- `~/.config/opencode/package.json`

### Plugins

- `opencode-browser`

### MCP servers

- `context7`
  - type: `remote`
  - url: `https://mcp.context7.com/mcp`
  - enabled: `true`
  - api key field: present in headers (`CONTEXT7_API_KEY`)
- `browsermcp`
  - type: `local`
  - command: `npx -y @browsermcp/mcp@latest`
  - enabled: `false`

### Installed skills (`~/.agents/skills`)

- `find-skills`
- `mobile-ios-design`
- `swift-composable-architecture`
- `swiftui-expert-skill`

### Additional skills (`~/.claude/skills`)

- `frontend-design`

## Exclusions

- No `backup/` folder is kept in this repository.
- No runtime/cache artifacts (`node_modules`, logs, temp files).
- No account/session data (`antigravity-accounts.json`, signature caches/logs).

## How To Refresh This Documentation

1. Re-check local files in `~/.config/opencode`, `~/.agents`, and `~/.claude`.
2. Update this `README.md` if plugins, MCPs, or skill lists changed.
3. Re-copy global `~/.config/opencode/AGENTS.md` into repo `AGENTS.md` if it changed.
4. Commit and push.
