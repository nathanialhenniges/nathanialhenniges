# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

GitHub profile README repository (`nathanhenniges/nathanhenniges`) — renders as the public profile at github.com/nathanhenniges. No application code, build system, or tests.

## Files

| File | Purpose |
|------|---------|
| `README.md` | Profile content (Markdown + inline HTML): cover image, social badges, about section, quote, auto-updated blog posts, Discord widget |
| `cover.png` | Hero banner (1584x396) |
| `.github/workflows/blog.yml` | GitHub Actions workflow that syncs blog posts into the README |

## Blog Post Workflow

- **Action:** `gautamkrishnar/blog-post-workflow` pulls from `https://www.mrdemonwolf.com/feed/`
- **Schedule:** Weekly (Sunday 00:00 UTC) + manual `workflow_dispatch`
- **Markers:** Content injected between `<!-- BLOG-POST-LIST:START -->` and `<!-- BLOG-POST-LIST:END -->` in README.md
- **Links:** Include UTM params (`utm_source=github&utm_medium=profile-readme&utm_campaign=blog-section&utm_content=blog-listings`)
- **Committer:** `NathanialHenniges` / `natanial.henniges@mrdemonwolf.com`

## Notes

- Nathan Henniges is **President of MrDemonWolf, Inc.** — GitHub org: https://github.com/MrDemonWolf | Website: https://www.mrdemonwolf.com
- Online alias across platforms: **mrdemonwolf**
- Services offered: Web Design & Development, Web Applications, SEO, Business Email Setup
- The README About Me section mirrors content from the mrdemonwolf.com about page — keep them in sync when updating
- No dependencies, no build commands, no tests
