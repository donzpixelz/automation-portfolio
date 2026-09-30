# Lead Intake & Human Handoff

**Example n8n workflow showing how multiple inbound channels can feed one shared qualification and routing process.**

> **Example architecture only.** This is a portfolio design example, not a currently deployed client system. No Meta, Instagram, WhatsApp, or other external credentials are connected.

## Workflow

```text
Meta Lead Ads ─┐
Instagram DM  ─┼→ Normalize Lead → Validate → Duplicate Check → Qualify
WhatsApp      ─┘                                  ↓
Webhook/Form  ────────────────────────────────────┘
                                                   ↓
                                      ┌────────────┴────────────┐
                                      ↓                         ↓
                               Auto response              Human handoff
                                      ↓                         ↓
                                      └────────→ Record / CRM ←─┘
```

The design keeps channel-specific input separate from the shared business logic. After normalization, the same validation, duplicate check, and qualification process can handle every lead.

Qualified leads can take an automated path when appropriate, or move to a human when the situation needs judgment. Both paths end in a durable record/CRM step.

## Built with

**n8n · Webhooks · APIs · routing · CRM integration · human-in-the-loop**

**Important:** This diagram demonstrates workflow design and n8n thinking. It does not claim that these integrations are live, that credentials exist, or that this exact workflow has been deployed.
