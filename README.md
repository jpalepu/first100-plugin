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

The plugin adds four First100 MCP servers (`first100-core` for brand memory, posts and the growth loop; `first100-seo` for search and AI visibility; `first100-autopilot` for blog publishing and workflows; `first100-outreach` for finding customers and email) and five skills (below). Each skill names the server it needs.

Not on Claude Code? claude.ai and Claude Desktop take `https://firsthundred.app/api/mcp` as a custom connector; ChatGPT (paid plans) adds it under Plugins after turning on Developer mode (OAuth, no key); Codex, Cursor, Windsurf and Zed instructions are at https://firsthundred.app/docs/clients.

## Skills

- `content-plan`: plan, write, review and queue posts.
- `blog-post`: research, write and publish a blog post that earns links and AI citations (GitHub, WordPress, Ghost, Webflow or a hosted blog).
- `growth-review`: weekly review of what worked, the funnel, and what to change.
- `morning-brief`: the daily page: numbers, replies to make now, the post to publish.
- `workflows`: set up, check or run workflows that write, publish and announce on a schedule.

The skills are thin on purpose: the rules, targets and the account's own performance findings come from the First100 server at run time.
