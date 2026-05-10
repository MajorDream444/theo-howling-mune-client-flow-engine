# Implementation Plan

## Phase 0 - Project Setup

- Create dedicated Theo repo/folder.
- Create source, docs, schemas, prompts, skills, app, automations, assets, and client status structure.
- Add `.env.example` and `.gitignore`.
- Link from Client Clarity OS.

## Phase 1 - Clarity / Source Consolidation

- Add transcript and PDF-derived markdown into `source/`.
- Update `docs/source-index.md`.
- Run blueprint extraction prompt.
- Human-review founder profile, doctrine, ICP, offer, and public claims.

## Phase 2 - Front Door

- Draft landing copy.
- Build first landing page.
- Mobile QA.
- Confirm CTA, fit/not-fit, and application path.

## Phase 3 - Intake + CRM

- Build intake form from schema.
- Submit test payload.
- Create Airtable lead.
- Route lead and update CRM fields.
- Trigger operator notification.

## Phase 4 - Close Flow + Stripe

- Create proposal/SOW from approved terms.
- Create Stripe Milestone 01/02/03 links.
- Wire webhook payment status.
- Confirm build task activation only after payment and approval.

## Phase 5 - Launch + Data Review

- Launch front door.
- Review first applications.
- Track route distribution, objections, close rate, and source quality.
- Decide whether to expand only after data exists.
