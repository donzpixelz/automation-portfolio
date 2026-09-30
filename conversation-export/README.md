# Conversation Export — Canonical

**Take an exact conversation request, resolve the correct record, export it, and verify the requested result.**

## Why it exists

A conversation export is only useful if it is the conversation that was actually requested. This workflow resolves the project and conversation identity before running the export, rejects ambiguity, and verifies the resulting branch.

## What it does

1. Receives an export request through a webhook.
2. Resolves the exact project/conversation identity.
3. Runs the proven export bridge.
4. Returns Markdown and exact conversation metadata.
5. Confirms that the current branch reaches the root.

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

**n8n · Webhooks · REST APIs · JSON · authenticated routing · verification**

## Inspect

[Canonical workflow](https://github.com/donzpixelz/project-gateway/blob/main/control-plane/registry.json) — the registered Gateway capability identifies this workflow as the canonical conversation-export route.

[Portfolio source evidence](https://github.com/donzpixelz/donzpixelz/tree/main/portfolio/proof)
