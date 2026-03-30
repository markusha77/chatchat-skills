---
id: create-skill-file
name: Create Skill File
description: Write and review skill file documentation with clear frontmatter, examples, boundaries, and maintenance expectations.
category: Documentation
requires: []
examples:
  - "Help me create a skill file that follows the repository format and reads clearly."
  - "Review this skill file draft for frontmatter, examples, boundaries, and instruction quality."
---

# Create Skill File

Use this skill when the user is authoring or reviewing a skill file and needs it to be structurally correct, readable, and aligned with repository expectations.

## Start By Clarifying
- What problem the skill is supposed to solve.
- Whether the skill is guidance-only or depends on supported backend tooling.
- Which audience will use the skill and what prompts should trigger it.
- What examples best show the intended use without being redundant.
- What boundaries should be explicit so the skill does not overclaim capability.

## Workflow
1. Define the skill's purpose, scope, and intended user requests.
2. Write compliant frontmatter with `id`, `name`, `description`, `category`, `requires`, and `examples`.
3. Draft instructions around user outcomes, decision points, and common failure modes.
4. Add examples that demonstrate real usage patterns rather than generic filler.
5. Review the file for overlap, unsupported claims, and missing boundaries before treating it as ready.

## Good Output
- Skill-file structure with correct frontmatter.
- Clear instructions that explain when and how the skill should help.
- Examples that improve discoverability and expectation-setting.
- Boundary notes that prevent hidden-tool or hidden-state assumptions.
- Review notes on overlap, clarity, or maintenance risk.

## Common Pitfalls
- Writing a skill name without giving the body a real workflow or job to do.
- Using generic examples that could fit any skill in the repo.
- Leaving unsupported backend assumptions in a guidance-only skill.
- Creating a skill that duplicates an existing stronger canonical skill.
- Treating frontmatter as valid while missing the actual reader-facing clarity.

## Boundaries
- Do not imply nonexistent tools, local services, hidden state, or privileged integrations.
- Prefer clear scope, examples, and behavioral guidance over placeholder boilerplate.
