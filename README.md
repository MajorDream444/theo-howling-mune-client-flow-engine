# Theo / Howling Mune Client Flow Engine V1

Dedicated implementation scaffold for Theo / Howling Mune inside the broader Client Clarity Intake OS.

## What Theo V1 Is

Theo V1 is the first clean revenue layer for Howling Mune:

- one clear front door
- one intake/application flow
- one routing logic
- one lead tracker
- one close pathway
- one first paid offer path

The project exists so aligned clients can understand the work, apply, get routed properly, and move toward paid engagement without relying on referrals, scattered DMs, or Theo manually explaining the work every time.

## What It Is Not

- Not the full Howling Mune operating system.
- Not a retreat, practitioner, facility, or community platform.
- Not an automated pricing engine.
- Not a public-claims generator.
- Not a replacement for Major/human review of strategy, pricing, claims, or client-facing language.

## Strategic Status

Theo already has real lived authority, proof from 1:1 and group work, and a coherent body of work around self-relationship, embodiment, healing, silence, contemplation, and returning people to themselves.

The missing piece is the pathway around the work: a front door, qualification path, CRM, close sequence, and paid engagement route. Howling Mune remains the umbrella brand. The first room opened is the flagship entry offer, currently held for human review as Identity Reset / Visual Rebirth or the final agreed equivalent.

## Implementation Status

This repo is the dedicated Theo implementation project. The generic Client Clarity OS remains the system spine; this repo is the first concrete client implementation example.

Current state:

- markdown/spec layer created
- source slots created for transcript, blueprint, and strategic documents
- schemas created for intake, routing, and CRM
- prompts created for landing copy, intake generation, lead routing, close scripts, content rhythm, and blueprint extraction
- automation connection docs created for Airtable, Notion, Stripe, and n8n
- app folders are placeholders for the first front-door and intake build

## System Loop

```text
Client record in Airtable
-> Intake / source material
-> Blueprint extraction
-> Human review
-> Proposal / SOW
-> Stripe payment
-> Build tasks
-> Front door + intake + CRM
-> Launch / optimization
```

## Required Environment Variables

Copy `.env.example` to `.env` for local wiring. Do not commit `.env`.

- `AIRTABLE_API_KEY`
- `AIRTABLE_BASE_ID`
- `AIRTABLE_CLIENTS_TABLE_ID`
- `AIRTABLE_INTAKE_RESPONSES_TABLE_ID`
- `AIRTABLE_BLUEPRINT_OUTPUTS_TABLE_ID`
- `AIRTABLE_ASSETS_TABLE_ID`
- `AIRTABLE_BUILD_TASKS_TABLE_ID`
- `NOTION_API_KEY`
- `NOTION_THEO_DOSSIER_PAGE_ID`
- `STRIPE_SECRET_KEY`
- `STRIPE_WEBHOOK_SECRET`
- `STRIPE_PRICE_M01`
- `STRIPE_PRICE_M02`
- `STRIPE_PRICE_M03`
- `TELEGRAM_BOT_TOKEN`
- `TELEGRAM_CHAT_ID`
- `APP_BASE_URL`

## Manual Test Flow

1. Create or confirm Theo client record in Airtable.
2. Confirm source files are indexed in `docs/source-index.md`.
3. Run blueprint extraction against source material and validate human-review notes.
4. Generate draft landing page copy and intake questions.
5. Submit a test intake payload matching `schemas/intake/theo-intake.schema.json`.
6. Classify route against `schemas/routing/theo-routing.schema.json`.
7. Create or update a Theo lead record matching `schemas/crm/theo-lead.schema.json`.
8. Confirm notification and close-flow task are created.
9. Confirm Stripe milestone links are present in test mode before sharing.
10. Require Major/human approval before final copy, pricing, claims, or launch.

## Build Order

1. Phase 0: project setup and source consolidation
2. Phase 1: clarity docs and blueprint extraction
3. Phase 2: front door landing page
4. Phase 3: intake form and Airtable CRM write
5. Phase 4: close flow and Stripe milestone path
6. Phase 5: launch QA and data review

## Human-Review Gates

- Pricing and commercial terms
- Public transformation claims
- Final landing page copy
- Proposal/SOW language
- Stripe payment link selection
- Any move beyond V1 into groups, retreats, practitioner systems, facilities, or full OS features
