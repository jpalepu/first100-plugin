---
name: content-plan
description: Plan, write, review and queue social posts through First100. Use when the user asks to plan content, fill the calendar, schedule posts, or "post about X this week".
---

# Content plan

Needs the `first100-core` MCP server (https://firsthundred.app/api/mcp/core).

First100 holds the brand memory, the writing rules, the account's own performance findings, the slots, the drafts and the queue. Follow its instructions, not generic advice.

1. Run the `plan_content` MCP prompt (or call `get_content_context`, then `what_worked`) and follow the steps it returns. The context carries the rules and what this account's numbers say.
2. Write one post per slot. Before saving each one, call `review_post` and apply every fix until the verdict is `ready`.
3. Save with `save_drafts`, then `approve_posts` after the user says yes (unless auto-publish is on).

If a tool says an account is not connected or needs reconnect, stop and send the user to the URL in the message.
