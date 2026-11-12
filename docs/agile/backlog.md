# Prioritized backlog

Status reflects repository preparation, not customer or runtime readiness. P0 is needed for the next decision; P1 follows it; P2 is deferred. Effort: S under two hours, M two to six, L more than six; all estimates.

| ID | Priority | Story and outcome | Acceptance criteria | Dependency | Status |
|---|---|---|---|---|---|
| PLAN-01 | P0 | Preserve operating model | Complete source plan linked; hypotheses labeled | None | Review |
| PLAN-02 | P0 | Make roles reusable | Shared policy and six role files; reviewer separate | PLAN-01 | Review |
| PLAN-03 | P0 | Establish Agile delivery | Roadmap, ready/done rules, backlog and sprint linked | None | Review |
| PLAN-04 | P0 | Standardize handoffs | Task, assessment, proposal and owner packet templates | PLAN-01 | Review |
| PLAN-05 | P0 | Specify quality checks | Failure and authority scenarios with expected results; not claimed passed | PLAN-02 | Review |
| DEC-01 | P0 | Select first buyer and offer | Greg records buyer, problem, price hypothesis and exclusions | PLAN-01 | Todo |
| REH-01 | P1 | Draft fictional assessment | Synthetic notes, three recommendations, source assumptions | DEC-01 | Todo |
| REH-02 | P1 | Draft fictional proposal | Two-system scope, acceptance, exclusions and pricing | REH-01 | Todo |
| REH-03 | P1 | Review rehearsal independently | Critique, revised version and review outcome recorded | REH-02 | Todo |
| VAL-01 | P1 | Design five-prospect test | Prospect criteria and conversation questions; no sends | DEC-01 | Todo |
| EXP-01 | P2 | Assess invoice pilot | Thirty-invoice scope, accuracy and effort decision rules | DEC-01 | Review of plan only |
| ARCH-01 | P1 | Inventory current tools | Current Paperclip and access capabilities verified under authorized scope | Explicit inspection scope | Blocked |
| ARCH-02 | P1 | Choose runtime | Compare existing stack with fresh option against control requirements | ARCH-01 | Blocked |
| BUILD-01 | P2 | Enforce authority and budgets | Gateway denies unapproved writes; costs bounded; audit evidence | Implementation authorization, ARCH-02 | Blocked |
| BUILD-02 | P2 | Implement internal workflow | Synthetic fixtures, recovery and duplicate tests pass | BUILD-01 | Blocked |
| PILOT-01 | P2 | Deliver one paid pilot | Accepted scope, trusted payment and acceptance record | BUILD-02, customer approval | Blocked |

Planning stories PLAN-01 through PLAN-05 are S or M. Rehearsal stories are M. Architecture and build stories need re-estimation after inventory; no delivery date is assigned.

No story may be marked Done solely because it appears in this table. Review completion must be recorded in the PR or sprint log.
