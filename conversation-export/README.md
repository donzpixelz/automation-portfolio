# Conversation Export — Canonical

**Take an exact conversation export request outside the Chrome extension, resolve the correct project and conversation, perform the export through the canonical workflow/API path, and verify the result.**

## Why it exists

BranchBind handles the browser-side case while you are viewing a conversation in Chrome. Conversation Export handles a different job: an exact export request comes in from the CLI, web app, or Desktop-side tooling, and the system resolves the requested record before exporting it.

## What it does

1. Receives an exact export request outside the Chrome extension.
2. Resolves the correct project/conversation identity and rejects ambiguity.
3. Performs the export through the canonical workflow/API path.
4. Returns Markdown and exact conversation metadata.
5. Verifies that the requested branch reaches the root.

## Verified result

A successful production execution on **2026-09-29**:

| Result | Verified value |
| --- | --- |
| Execution | `1759` |
| Status | `success` |
| Trigger | webhook |
| Selected turns | **384** |
| Markdown result | **268,184 bytes** |
| Full branch root | **confirmed** |
| Current path | resolved from ChatGPT `current_node` |

The workflow is `vmHnoXvpNXMqBWQh`, **Conversation Export — Canonical**.

## Built with

**CLI · web app · Desktop tooling · REST APIs · JSON · n8n**

n8n is the implementation and proof layer for the canonical workflow; it is not the product identity.

## Inspect

[Canonical workflow](https://github.com/donzpixelz/project-gateway/blob/main/control-plane/registry.json) — the registered Gateway capability identifies this workflow as the canonical conversation-export route.

[Portfolio source evidence](https://github.com/donzpixelz/donzpixelz/tree/main/portfolio/proof)
