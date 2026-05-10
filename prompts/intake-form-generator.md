# Intake Form Generator Prompt

Generate a Theo / Howling Mune intake form from `schemas/intake/theo-intake.schema.json`.

Rules:

- Ask only what is needed for qualification and routing.
- Keep questions reflective but not exhausting.
- Include consent.
- Do not ask for sensitive clinical detail.
- Do not imply guaranteed outcomes.

Return:

- field label
- field help text
- input type
- required status
- routing relevance
