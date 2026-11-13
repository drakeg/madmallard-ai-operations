# Platform readiness and read only inventory plan

No current environment has been inspected for this project. Existing Paperclip and agent names come from prior discussion and must not be treated as current configuration.

## Sanitized inventory fields

| Area | Evidence to request during authorized inspection | Acceptance question |
|---|---|---|
| Existing runtime | Version, deployment method and documentation references | Can existing installation support the workflow? |
| Agent identities | Names, assigned duties and tool scopes, without secrets | Can roles be separated without disrupting existing work? |
| Queue | Persistence, restart behavior and task schema | Can a task resume without repeating writes? |
| Tools | Read, draft and write scopes and authorization model | Can prohibited actions be blocked outside prompts? |
| Review | Assignment and evidence storage | Can an author be prevented from self-approval? |
| Budget | Provider billing method and cap enforcement | Are estimated costs reserved before calls? |
| Data | Client isolation, storage and retention | Can each task access only its permitted records? |
| Recovery | Audit records, retry rules, pause control | Can uncertain writes be reconciled and new work stopped? |

Collect configuration summaries or redacted evidence, never raw tokens, environment dumps, customer payloads or confidential logs in Git. Do not probe a host or signed-in session without an authorized inspection scope. Record unknown for unavailable evidence.

## Platform decision worksheet

Candidates: retain existing Paperclip; fresh framework if existing controls cannot meet requirements; manual instruction-profile rehearsal while requirements remain uncertain.

For each required control, record supported evidence, missing capability, implementation effort estimate, recurring cost estimate and accountable owner. Labels: verified supported, needs implementation, unavailable or unknown. Do not score unknown as supported.

Preferred decision sequence: inspect existing tools, identify specific gaps, estimate the smallest remediation, then compare a fresh option. No candidate has been selected or benchmarked here. Model selection and pricing need fresh verification during actual design.

## Proposed initial implementation boundary for later approval

One internal workflow, synthetic data, one active task, four predefined roles, no outbound messaging, no production client credentials. Build only task records, scoped tool policies, budget accounting, review routing, audit trail and evaluation fixtures in an isolated environment. This is a draft scope, not permission to build.

Before requesting implementation approval, provide exact environment, artifacts to change, dependency versions, cost ceiling, acceptance tests, failure recovery and rollback. State separately whether inspection, coding, model API usage and local execution are authorized. No deployment permission is implied by approval of documentation.
