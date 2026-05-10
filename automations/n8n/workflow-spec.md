# n8n Workflow Spec

## Workflow A: Intake Submission -> Airtable Lead

Trigger: Theo intake form submission.

Steps:

- validate payload against intake schema
- create Airtable intake response
- create or update lead/client record
- store source and consent
- return confirmation

## Workflow B: Airtable Lead -> Route + Notification

Trigger: new or updated intake response.

Steps:

- classify route
- write route outcome to Airtable
- set next action
- notify operator through approved channel
- mark manual review when needed

## Workflow C: Payment Received -> Client Status / Build Task Activation

Trigger: Stripe webhook payment success.

Steps:

- verify webhook
- match milestone metadata
- update payment status
- activate build tasks only if proposal/SOW and human approval are present
- notify operator

## Workflow D: Blueprint Data -> Dossier Generation

Trigger: reviewed blueprint output.

Steps:

- generate or update Notion dossier
- link source records
- write dossier URL to Airtable
- leave proposal/pricing fields in human-review state

## Production Rule

Do not enable production triggers until test records, writebacks, and notifications are verified.
