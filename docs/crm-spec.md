# CRM Spec

## Airtable Lead Fields

| Local field | Airtable-ready field | Notes |
| --- | --- | --- |
| `lead_name` | Lead Name | Required |
| `email` | Email | Required when available |
| `whatsapp` | WhatsApp | Preferred close channel |
| `location` | Location | Include Bali/location context where relevant |
| `source` | Source | Referral, content, DM, event, direct, partner |
| `pathway` | Pathway | Route outcome |
| `readiness` | Readiness | low, medium, high, urgent |
| `budget` | Budget Comfort | human-reviewed, not auto-priced |
| `status` | Status | new, reviewing, contacted, fit_call, proposal_sent, paid, nurture, closed_lost |
| `last_contact` | Last Contact | Date |
| `next_action` | Next Action | Operator action |
| `close_probability` | Close Probability | 0-100 estimate |
| `offer_interest` | Offer Interest | Healing, photography, hybrid, group, partner |
| `notes` | Notes | Freeform operator notes |

## Status Rule

No lead becomes `paid` without verified payment status. No pricing or final offer terms are auto-finalized from the CRM.
