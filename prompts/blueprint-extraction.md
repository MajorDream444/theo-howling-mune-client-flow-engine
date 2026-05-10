# Blueprint Extraction Prompt

Extract a structured Theo / Howling Mune blueprint from preserved source files.

Inputs:

- `source/transcripts/theo-vision-call-2026-04-21.md`
- `source/blueprints/theo-foundational-blueprint.md`
- `source/blueprints/theo-blueprint-luxury.md`
- `source/strategic/*.md`

Rules:

- Do not invent client facts.
- Separate doctrine from offer.
- Separate Phase 1 from future vision.
- Mark unavailable or uncertain source claims as `needs_source`.
- Pricing, public claims, and proposal terms require human review.

Return sections:

- founder profile
- doctrine
- ICP
- offer architecture
- phase 1 recommendation
- routing logic
- close flow
- deferred expansion
- human-review flags
