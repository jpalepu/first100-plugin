---
name: blog-post
description: Research and write a blog post built to earn links and AI citations through First100. Use when the user asks for a blog post, an article, a guide, or content to outrank a competitor.
---

# Blog post

Run the `write_blog` MCP prompt with the topic (and competitor URLs if the user names any) and follow it: `research_blog` for the brief and targets, write the markdown, `review_blog` until the verdict is `ready`. Ask the user for the company-specific facts the brief marks as missing rather than inventing them.
