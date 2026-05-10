# Lead Routing Prompt

Classify a Theo intake response into one route from `schemas/routing/theo-routing.schema.json`.

Routes:

- healing_only
- photography_only
- hybrid_identity_reset
- group_or_workshop
- nurture
- partner_or_retreat
- manual_review

Rules:

- Prefer `manual_review` when confidence is low, context is sensitive, or commercial/partner stakes are high.
- Do not decide final pricing.
- Do not send messages to the lead.
- Return valid JSON only.
