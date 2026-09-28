---
name: workflows
description: Set up, check or run First100 workflows that write, publish and announce content on a schedule. Use when the user wants something to happen automatically every day or week (a daily blog post, weekly announcements, a weekly search report) or asks what their workflows did.
---

# Workflows

Needs the `first100-autopilot` MCP server (https://firsthundred.app/api/mcp/autopilot).

Call `list_workflows` first: it shows the brand's workflows with each block's last result, and the templates. To create one, pick the template that matches the request and call `create_workflow` with the user's schedule, language and platforms; confirm with the user before creating one that publishes, since workflows run fully automatically unless they include an approval step. `run_workflow` runs one now. Point the user to https://www.firsthundred.app/dashboard/workflows to change blocks on the canvas.
