# Proposed technical design

Document only. No code, accounts, containers, schedules or services were created. Platform and deployment selection are intentionally deferred until actual capability inspection is authorized.

## Data path

Existing form → authenticated intake → validation and durable work record → idempotent tracking write → response-template field → awaiting human review.

The intake and worker are proposed integration components, not additional customer business systems. Their hosting, logs and credentials still need explicit approval and cost disclosure. There is no email API connection.

## Minimal record

submission_id, received_at, synthetic_client_id, name, email, service_interest, inquiry_text, processing_status, draft_text, last_error_code, attempt_count, target_record_id. Payload size and allowed characters must be specified after inspecting the real form. Retain only necessary fields under the agreed policy.

## Proposed state transitions

Received → validated → write_pending → awaiting_review. Invalid input → exception. Transient failure → retry_pending. Ambiguous target write → reconcile_pending. Exhausted attempts → needs_owner. These are design states; no controller exists yet.

## Duplicate and failure behavior

Use client ID plus immutable submission ID as the unique work key. Enforce uniqueness in durable storage. Store a content fingerprint; a replay with changed content becomes a conflict for review, not an automatic overwrite. Use the target's supported upsert or reconcile by the unique external ID. If the target cannot support safe reconciliation, redesign before committing to the pilot.

Authenticate inbound requests, validate timestamps and signature where supported, limit payload size and rate, and keep secrets out of logs. Retry only transient errors with a bounded schedule; reconcile uncertain writes before retrying. Preserve the native form record as the recovery source. Define recovery ownership and operating hours in the real scope.

## Acceptance fixture design

Normal submission, duplicate replay, changed-content replay, missing email, invalid signature, stale request, expired target credential, target timeout after write, worker restart and instruction-like text in an inquiry. For each, record expected target rows, status, draft behavior and permitted actions. Actual runtime testing: not performed.

## Release and rollback proposal

Before release, obtain a reviewed version, access approval, cost ceiling and client demonstration plan. For rollback, disable the integration route, preserve the original form records, reconcile in-flight records and return to manual entry. Do not delete records to conceal a failed run. Later activation is outside this sprint.
