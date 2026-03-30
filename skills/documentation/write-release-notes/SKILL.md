---
id: write-release-notes
name: Write Release Notes
description: Write release notes with clear impact, compatibility notes, rollout context, and reader actions.
category: Documentation
requires: []
examples:
  - "Draft release notes that explains impact, migration notes, and known issues clearly."
  - "Review release notes so readers can tell whether they are affected and what to do next."
---

# Write Release Notes

Use this skill when the user needs release notes so readers understand what changed, why it matters, and what they need to do next.

## Start By Clarifying
- Who the release notes are for and what they care about most.
- Which changes are user-visible, operationally significant, or compatibility-sensitive.
- Whether migrations, deprecations, or rollout caveats need explicit treatment.
- What risks, known issues, or support guidance should be surfaced.
- How much implementation detail helps rather than distracts.

## Workflow
1. Collect the meaningful changes and group them by reader impact, not commit chronology.
2. Highlight features, fixes, breaking changes, and operational notes separately where useful.
3. Add migration or upgrade guidance wherever readers may need to take action.
4. Call out known issues, rollout caveats, and audience-specific warnings honestly.
5. Review the notes for clarity, completeness, and whether affected readers can recognize themselves.

## Good Output
- Release summary tailored to the intended audience.
- Grouped notes by impact or change type.
- Migration, rollback, or compatibility notes.
- Known issues or rollout caveats that should not be hidden.

## Common Pitfalls
- Copying commit messages instead of explaining reader impact.
- Burying breaking changes among minor fixes.
- Leaving users unsure whether they need to act.
- Overstating rollout completeness or stability without confirmation.

## Boundaries
- Do not imply a change is fully rolled out unless the user confirms it.
- Prefer impact-focused communication over changelog noise.
