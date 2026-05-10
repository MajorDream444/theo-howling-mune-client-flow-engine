# Stripe Milestone Flow

## Milestone 01

Purpose: first payment that activates build start.

Trigger:

- signed/accepted SOW
- approved commercial terms
- Stripe link sent
- payment received

Result:

- Airtable Payment Status updated
- Build Tasks activated
- build begins within 48 hours

## Milestone 02

Purpose: mid-build or second agreed payment.

Final amount and timing require approved SOW terms.

## Milestone 03

Purpose: final agreed payment or launch/completion milestone.

Final amount and timing require approved SOW terms.

## Metadata Fields

- `client_slug=theo-howling-mune`
- `project=theo-howling-mune-client-flow-engine`
- `milestone=m01|m02|m03`
- `airtable_client_record_id`
- `proposal_version`
- `human_approved=true|false`

## Webhook Behavior

On successful payment:

- verify webhook signature
- match client and milestone metadata
- update Airtable payment status
- add payment timestamp
- activate approved build tasks if Milestone 01
- notify operator

## Rule

Stripe links and prices must be human-reviewed. Code must not select or finalize the `$4,500` or `$6,500` build fee automatically.
