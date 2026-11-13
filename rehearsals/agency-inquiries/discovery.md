# Synthetic discovery notes

Fixture ID: SYN-AGENCY-001. Fictional business: Example Agency, six staff. Source: authored scenario, not an interview. All quantities below are assumptions chosen for arithmetic and scope review.

## Current process

The owner receives website inquiry notifications, copies details into a tracking sheet and writes the first follow-up. The existing web form assigns an immutable submission ID and timestamp and supports configurable delivery to an API endpoint; these capabilities must be verified on a real customer's platform.

| Input | Fixture assumption |
|---|---:|
| Inquiries weekly | 20 |
| Manual entry per inquiry | 4 minutes |
| Follow-up preparation per inquiry | 3 minutes |
| Review of an automated draft | 2 minutes |
| Weekly exception allowance after automation | 10 minutes |
| Owner time valuation for illustration | $50/hour |

An assistant occasionally repeats an entry because there is no submission-ID check. No missed-sales percentage or lost revenue is assumed. The owner wants a consistent tracking record and a suggested response, with human approval before any message goes out.

## Proposed pilot boundaries

Two systems: the existing form platform and a tracking workspace. The response draft is a field in the tracking record, not an email draft in a third application. Human review and manual sending happen outside the integration. No mailbox, CRM, calendar, payment or booking integration is included.

The inquiry may contain a name, email, service interest and free text. Production use needs permission and a retention agreement. Rehearsal examples use synthetic names and reserved example.com addresses only.

## Unresolved discovery questions

Does the form support stable IDs, signed webhooks and safe replay? Does the tracking platform support unique keys or safe upserts? Which subscriptions are required? Who may review records? What happens to deletions and opt-outs? Does the form already send an acknowledgment? What deadline and response hours does the owner expect?

None of these questions is resolved by the fictional fixture. Unsupported capabilities block a fixed-price production commitment.
