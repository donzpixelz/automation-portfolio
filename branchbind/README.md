# BranchBind

**Save the exact ChatGPT conversation branch you are looking at and preserve it cleanly to GitHub or download it.**

## Why it exists

ChatGPT conversations can contain sibling branches that are not part of the path currently being viewed. BranchBind preserves the active branch instead of treating the whole conversation record as one flat history.

## What it does

- Loads the authenticated conversation from the ChatGPT page context.
- Reconstructs the active path from `current_node`.
- Exports clean Markdown.
- Downloads through Chrome, archives through a narrow GitHub Worker, or does both.
- Refreshes automatically as ChatGPT navigation changes.

Example output:

```text
bb--ai-unfuck--dev-nav-d.md
```

## Built with

**Chrome MV3 · JavaScript · ChatGPT page-context requests · Cloudflare Worker · GitHub**

The extension uses only `activeTab`, `scripting`, and `downloads` permissions. GitHub credentials remain server-side.

## Inspect

[BranchBind source repository](https://github.com/donzpixelz/branchbind) — private source repository; portfolio proof is based on the current verified source state.

[Sanitized proof](https://github.com/donzpixelz/donzpixelz/blob/main/portfolio/proof/branchbind.md)
