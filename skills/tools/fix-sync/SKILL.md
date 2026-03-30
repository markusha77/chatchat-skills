---
id: fix-sync
name: Fix Sync
description: Diagnose and remediate synchronization failures across services, workers, queues, or replicas with safe recovery and verification steps.
category: Tools
requires: []
examples:
  - "Diagnose delayed event processing causing stale read models between API and worker services."
  - "Fix bi-directional sync conflicts and define idempotent replay procedures."
---

# Fix Sync

Use this skill when data or state has drifted between systems and the user needs a safe way to diagnose the break, recover consistency, and reduce recurrence risk.

## Clarify First
- What system is the source of truth.
- Which downstream systems or replicas are expected to stay in sync.
- How much lag is acceptable before it becomes an incident.
- Whether the break is caused by missing events, duplicate processing, bad conflict resolution, or manual patching.
- What proof would show the systems are reconciled again.

## Investigation Priorities
- Bound the incident by time window, entities affected, and business impact.
- Trace the sync path from producer through transport to consumer and persistence.
- Check ordering, retries, idempotency, and dead-letter behavior before replaying anything.
- Distinguish missing data from delayed data from conflicting data.
- Prefer reversible, scoped remediation over broad repair attempts.

## Recovery Guidance
- Replay only when idempotency and scope are understood.
- Backfill missing records in deterministic batches.
- Use explicit conflict rules instead of silent last-write surprises.
- Verify parity through both sampled records and aggregate checks.
- Add monitors for lag, replay failures, and reconciliation drift after the immediate fix.

## Common Failure Modes
- Replaying events into consumers that are not actually idempotent.
- Manual data fixes that bypass the sync path and create new drift.
- Ignoring DLQ growth until the incident becomes much larger.
- Relying on timestamps whose ordering is not trustworthy.
- Declaring resolution before proving both systems match again.

## Good Output
- Drift summary and likely sync stage where failure began.
- Safe remediation sequence in order.
- Validation checks to prove reconciliation.
- Preventive controls such as lag alerts, idempotency enforcement, or reconciliation jobs.
- Conflict strategy rationale where multiple writes can compete.

## Boundaries
- Do not recommend broad replay or mutation without first surfacing idempotency and rollback concerns.
- Prefer investigation structure, recovery sequencing, and verification logic over pretending to inspect live systems directly.
