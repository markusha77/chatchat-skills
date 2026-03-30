---
id: executing-plans
name: Executing Plans
description: Turn approved plans into controlled execution steps with sequencing, decision gates, risk tracking, and verifiable progress.
category: Tools
requires: []
examples:
  - "Convert a multi-phase migration plan into tracked execution steps with verification gates."
  - "Run an agreed delivery plan while managing dependencies, blockers, and rollback decisions."
---

# Executing Plans

Use this skill when the user already has an agreed plan and needs help turning it into disciplined execution rather than a loose status narrative.

## Start By Clarifying
- What has already been approved versus what is still uncertain.
- Which milestones are truly dependent on earlier work.
- What evidence counts as done for each stage.
- Which blockers would change sequence, scope, or rollout safety.
- What rollback or pause conditions matter most.

## Execution Principles
- Break plans into milestones with explicit done criteria.
- Sequence by dependency and risk, not optimism.
- Keep verification gates close to the work they validate.
- Surface blockers early with owner, impact, and next decision point.
- Re-baseline the plan when assumptions change materially.

## Good Execution Structure
- Milestones with owner, status, and acceptance criteria.
- Critical-path tasks and dependency notes.
- Verification gates for builds, tests, rollout checks, or review steps.
- Blocker log with severity, mitigation, and escalation timing.
- Next actions tied to evidence rather than vague progress labels.

## Decision Guidance
- Prefer smaller reversible increments over big-bang execution.
- Do not parallelize tasks that share the same risky dependency.
- Reduce scope before reducing verification.
- Treat rollout evidence as mandatory for high-impact stages.
- Mark work complete only when the acceptance criteria are demonstrated.

## Common Mistakes
- Tracking activity instead of outcome.
- Calling work done without proof tied to acceptance criteria.
- Letting blockers age without a clear owner or escalation path.
- Continuing with an outdated plan after scope or constraints changed.
- Compressing risky dependent work into one milestone for convenience.

## Good Output
- Execution summary with current status.
- Milestone-by-milestone progress and gates.
- Critical path and active blockers.
- Verification evidence needed next.
- Recommended next execution steps or re-baselining decisions.

## Boundaries
- Do not claim work is complete, validated, or shipped unless the user provides that evidence.
- Prefer execution structure, progress discipline, and risk framing over pretending to update external trackers automatically.
