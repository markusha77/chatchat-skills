---
id: netalertx-sample-data
name: NetAlertX Sample Data
description: Plan realistic, deterministic NetAlertX sample data for development, demos, and testing without leaking production-sensitive information.
category: Tools
requires: []
examples:
  - "Create anonymized device and alert data for local UI testing."
  - "Build a repeatable seed dataset for NetAlertX integration tests."
---

# NetAlertX Sample Data

Use this skill when the user needs believable NetAlertX development or demo data without exposing real production identities, devices, or histories.

## Clarify First
- Whether the dataset is for UI demos, automated tests, local development, or onboarding.
- Which entities matter most: devices, events, alerts, histories, or relationships.
- How much realism is needed versus how fast the dataset must load.
- Whether anonymized snapshots are acceptable or synthetic-only data is safer.
- What edge cases the data must exercise.

## Design Priorities
- Keep the dataset deterministic so test runs stay reproducible.
- Preserve structural realism without preserving sensitive details.
- Include enough volume and variation to exercise real UI and workflow paths.
- Model edge cases deliberately instead of hoping random generation produces them.
- Keep reset and reload behavior simple for repeated use.

## Good Dataset Guidance
- Define entity counts, time ranges, and severity distributions explicitly.
- Use fixed seeds for any generated values.
- Include normal, noisy, and pathological alert patterns.
- Validate schema compatibility whenever the product model changes.
- Document generation, load, verification, and reset steps together.

## Common Mistakes
- Using tiny toy datasets that never exercise filtering, pagination, or bulk states.
- Letting randomness change identifiers or counts between test runs.
- Missing privacy leaks in comments, metadata, or copied identifiers.
- Forgetting schema drift until seed data breaks after a migration.
- Generating so much data that the development feedback loop slows down.

## Good Output
- Sample-data plan with source strategy and entity coverage.
- Data quality checklist for determinism, privacy, and schema fit.
- Edge cases and distributions worth modeling.
- Load, verification, and reset workflow.
- Risks if anonymized snapshots are used instead of synthetic data.

## Boundaries
- Do not imply that real production data is safe to reuse without explicit anonymization review.
- Prefer data-shape guidance, coverage planning, and privacy constraints over pretending to generate or load datasets automatically.
