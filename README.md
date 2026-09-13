# First100 for Claude Code

This folder is the source of the Claude Code plugin marketplace. Publish it as its own public repository (for example `jpalepu/first100-plugin`) with this folder's contents at the repository root.

## Install

```
/plugin marketplace add jpalepu/first100-plugin
/plugin install first100@first100
```

Then export your key before starting Claude Code:

```bash
export FIRST100_API_KEY=f100_...   # from https://firsthundred.app/dashboard/keys
```

The plugin adds the First100 MCP server and three skills (below).

Not on Claude Code? claude.ai and Claude Desktop take `https://firsthundred.app/api/mcp` as a custom connector; ChatGPT (paid plans) adds it under Plugins after turning on Developer mode (OAuth, no key); Codex, Cursor, Windsurf and Zed instructions are at https://firsthundred.app/docs/clients.

## Skills

- `content-plan`: plan, write, review and queue posts.
- `blog-post`: research and write a blog post that earns links and AI citations.
- `growth-review`: weekly review of what worked, the funnel, and what to change.
- `morning-brief`: the daily page: numbers, replies to make now, the post to publish.

The skills are thin on purpose: the rules, targets and the account's own performance findings come from the First100 server at run time.
