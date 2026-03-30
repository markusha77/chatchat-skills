---
id: code-style
name: Code Style
description: Improve code readability and consistency by aligning naming, structure, formatting, and local conventions without losing sight of clarity.
category: Tools
requires: []
examples:
  - "Help me improve the style and readability of this code without changing behavior."
  - "What style issues matter here beyond automatic formatting?"
---

# Code Style

Use this skill when the user wants guidance on code style in the meaningful sense: readability, consistency, naming, structure, and local convention fit.

## Clarify First
- Which language and local style conventions apply.
- Whether the code is already constrained by formatter or linter rules.
- Which style issues are hurting comprehension most.
- Whether the goal is cleanup, consistency, or review feedback.
- How much structural change is acceptable without altering behavior.

## Style Priorities
- Prefer readability over cleverness.
- Keep naming aligned with the surrounding codebase.
- Use structure to make intent obvious.
- Reduce incidental complexity before polishing surface aesthetics.
- Let automated formatting handle trivia so humans can focus on clarity.

## What Good Style Guidance Includes
- Naming improvements where intent is unclear.
- Function and block structure that better matches the responsibility.
- Better local consistency with existing patterns.
- Removal of noise that obscures the important logic.
- Clear distinction between subjective preference and project convention.

## Common Mistakes
- Treating formatter output as the whole of code style.
- Chasing stylistic purity while leaving confusing control flow untouched.
- Renaming aggressively without improving understanding.
- Applying one preferred pattern everywhere regardless of local norms.
- Giving feedback that is impossible to prioritize or justify.

## Good Output
- Most important readability issues first.
- Naming or structural adjustments that would clarify intent.
- Convention mismatches worth fixing for consistency.
- Low-value nits only after higher-signal guidance.

## Boundaries
- Do not treat subjective preference as an objective defect.
- Prefer clarity, local consistency, and maintainability over style dogma.
