---
id: workflows-yaml-reference
name: Workflows YAML Reference
description: Create and maintain workflow YAML reference docs with accurate contracts, examples, edge cases, and version-aware detail.
category: Documentation
requires: []
examples:
  - "Create workflow YAML reference docs with examples, constraints, and edge-case coverage."
  - "Review workflow YAML reference docs for gaps in contracts, parameters, compatibility notes, or failure cases."
---

# Workflows YAML Reference

Use this skill when the user needs workflow YAML reference docs that readers can trust as a durable lookup source rather than a vague narrative summary.

## Start By Clarifying
- What entities, endpoints, fields, functions, or concepts are actually in scope.
- Which versions, compatibility boundaries, or deprecations matter.
- What inputs, outputs, defaults, and error cases readers most often misunderstand.
- Which examples are necessary to make the reference usable, not just complete.
- What surrounding guide material should be linked rather than duplicated.

## Workflow
1. Define the reference surface and group it into durable reader-facing sections.
2. Document contracts, required fields, defaults, side effects, and failure modes explicitly.
3. Add examples that show normal use, edge cases, and compatibility caveats.
4. Call out version boundaries, deprecations, and non-obvious constraints.
5. Review for omissions that would force readers back into code or guesswork.

## Good Output
- Reference structure by resource, concept, or API surface.
- Missing contract details, examples, or compatibility notes.
- Places where defaults, limits, or failure behavior need stronger explanation.
- Cross-links needed to connect reference material to task-oriented guides.

## Common Pitfalls
- Documenting names without documenting behavior or constraints.
- Skipping error cases because the happy path feels sufficient.
- Hiding version-specific caveats until readers hit production issues.
- Letting the reference drift from actual source behavior.

## Boundaries
- Do not imply undocumented behavior is guaranteed.
- Prefer precise contracts and examples over broad marketing-style wording.
