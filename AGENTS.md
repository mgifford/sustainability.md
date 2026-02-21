# AGENTS.md

This repository supports AI coding agents.

## Canonical instructions

The canonical, repo-specific instructions for AI contributors live in:

- `.github/copilot-instructions.md`

All agents (Copilot and non-Copilot) should treat that file as the primary source of truth for contribution behavior, scope, and quality standards.

## Fallback behavior

If any instruction source conflicts, follow this precedence:

1. Direct human maintainer instruction
2. `.github/copilot-instructions.md`
3. Local file conventions and existing project style

## Notes

- Keep changes minimal and request-scoped.
- Validate Markdown/YAML after edits.
- Prefer deterministic, low-compute solutions where feasible.

For AGENTS.md background and interoperability context, see:

- https://agents.md/
