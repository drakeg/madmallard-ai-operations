# Approval and cost clarification

This addendum clarifies the existing operating plan. Current owner instruction: continue no-cost testing; make no changes that incur costs. Proposed future $100 model and $50 platform allowances are estimates, not current authorization. Do not call paid APIs or assume credits make a paid operation free. Do not enable GitHub Actions, scheduled runtime jobs or other metered services as part of this review.

A task's approved status means an internal planning or review milestone only. It cannot authorize an external action. External actions require the separate trusted approval record and gateway described in the operating plan. A worker cannot create, change or consume its own approval record. Merging documentation is not a token to send, deploy, purchase or access customer data.

In a later implementation, approval creation must be restricted to an authenticated authorized human; artifacts and targets must match; version changes invalidate approval; concurrent consumption must be atomic to prevent duplicate actions. Revocation and owner pause must be checked immediately before an external action. These are requirements, not implemented behavior.

Cost checks must include nested jobs, retries, tool charges and minimum provider billing units. Reserve conservative maximum spend before a call; reconcile actual charges afterward. If cost is unknown or zero cannot be established under the current policy, do not start the operation. Report blocked with the smallest no-cost alternative.

Customer commitments require explicit scope, response hours, included support and change/overage pricing. Do not silently absorb unlimited work or send an invoice for extra work without agreed terms.
