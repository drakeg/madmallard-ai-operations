# Mad Mallard business portfolio

Keep independent business experiments together through a shared topic and this hub index. Do not combine customer data, secrets or unrelated runtime dependencies.

## Repository convention
- New offering repositories: `madmallard-business-<offering>`; private by default.
- Shared topic: `madmallard-business` (hub and offering repos).
- Add descriptive topics for technologies and buyer niche.
- Portfolio discovery: https://github.com/search?q=owner%3Adrakeg+topic%3Amadmallard-business&type=repositories (sign in to see private repositories).
- Do not rename existing repositories without checking remote URLs, CI, integrations and deployment references. Link them here first.

## Current index
| Offering | Repository | Stage | Buyer / paid offer | Demand evidence | Deployment |
| --- | --- | --- | --- | --- | --- |
| Business operating hub | [madmallard-ai-operations](https://github.com/drakeg/madmallard-ai-operations) | Planning and portfolio | Internal operating plans | No validated demand implied | Documentation only |
| Accessibility audit workbench | [madmallard-business-accessibility](https://github.com/drakeg/madmallard-business-accessibility) | MVP under review | Small agencies; three-page audit + manual review + one retest; $249 pilot hypothesis | None yet; price unvalidated | Docker; ECS/ECR and EKS configuration; no cloud deployment |

## New-entry checklist
Record offering owner, buyer/problem, narrowly scoped offer, source/repo/video links, dependency licenses and review date, estimated effort/cost, pilot price hypothesis, five prospect criteria, 48-hour stop/go test, technical validation evidence, limitations, next milestone and PR link. Record facts separately from estimates and promotional income claims.

Stage labels: idea → researched → demand test → prototype → paid pilot → operating → parked. Technical completion never advances demand-validation status by itself. No outreach, purchase, paid API activation or cloud deployment is implied by an index entry. Update the index when evidence changes; keep product-specific backlog and runbooks in the offering repository.
