---
id: harness-writing
name: Harness Writing
description: Develop test harness docs with step-by-step guidance, examples, troubleshooting, and update ownership.
category: Documentation
requires: []
examples:
  - "Create test harness docs with step-by-step workflows, examples, and troubleshooting."
  - "Audit test harness docs for missing validation steps, stale procedures, and weak edge-case guidance."
---

# Harness Writing

Use this skill when the user is building test harness docs and needs a guide that people can actually follow under normal work and edge conditions.

## Start By Clarifying
- What tasks the handbook should support from start to finish.
- Which readers are beginners versus experienced maintainers.
- What tooling, environment, or safety assumptions must be explicit.
- Which examples, troubleshooting paths, or validation steps are essential.
- How the handbook will stay aligned with reality as systems evolve.

## Workflow
1. Define the handbook scope and the task sequence readers need most.
2. Write the guide around workflows, checkpoints, and recovery paths rather than just concepts.
3. Add examples, troubleshooting cues, and validation steps for common failure modes.
4. Surface prerequisites, limits, and risky assumptions early.
5. Review for stale steps, missing edge cases, and unclear ownership.

## Good Output
- Task-oriented handbook structure.
- Examples, validation checkpoints, and troubleshooting sections worth adding.
- Risks or stale assumptions that make the current guide hard to trust.
- Update and ownership guidance for long-term maintenance.

## Common Pitfalls
- Explaining theory while leaving readers unable to execute the task.
- Omitting troubleshooting because the happy path seems obvious.
- Leaving commands, version assumptions, or paths to decay silently.
- Packing too many unrelated workflows into one handbook.

## Boundaries
- Do not present unchecked steps as validated procedure.
- Prefer practical workflows and failure handling over generic advice.
