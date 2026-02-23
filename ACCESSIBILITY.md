# ACCESSIBILITY.md

> Project policy for inclusive, usable, and standards-aligned digital experiences.

This file is designed to inform `AGENTS.md` and all product/engineering decisions.

## Scope

Applies to:
- Content structure and navigation
- UI components and interactions
- Forms and error handling
- Media and data visualizations
- Documentation and support content

## Core requirements

### 1) Conformance baseline
- Target WCAG 2.2 AA (or stricter where required).
- Document known accessibility gaps with owner and timeline.
- Prevent new critical blockers from shipping.

### 2) Accessibility as a release criterion
- Accessibility checks are required in CI for changed interfaces.
- Keyboard access, focus visibility/order, semantic structure, and contrast are mandatory checks.
- Do not merge regressions in critical accessibility issues without explicit approved exception.

### 3) Inclusive implementation defaults
- Prefer semantic HTML before ARIA.
- Ensure meaningful names/labels/instructions for controls.
- Provide text alternatives for non-text content.
- Ensure content works across input methods, zoom, and small screens.
- Avoid motion/interaction patterns that can create barriers.

### 4) Testing and governance
- Use automated tooling plus targeted manual checks.
- Track accessibility issues with consistent labels and severity.
- Keep component patterns documented so AI/humans reuse accessible implementations.

## Pull request checklist

Each PR should include:
- Accessibility impact (`improves` / `neutral` / `regresses`)
- Checks run and key results
- Any exceptions with issue link, owner, and expiry date

## Suggested CI checks

- Accessibility linting for markup/components
- Automated checks for changed pages/components
- Contrast checks
- Keyboard/focus checks for interactive UI
- Merge gate on critical violations

## Trusted references

- https://www.w3.org/TR/WCAG22/
- https://www.w3.org/WAI/fundamentals/accessibility-intro/
- https://www.w3.org/WAI/standards-guidelines/aria/
- https://github.com/mgifford/ACCESSIBILITY.md

## Agent instruction snippet

Add to `AGENTS.md` or system prompts:

> Read `ACCESSIBILITY.md` before changing UI/content. Use semantic patterns, preserve keyboard and screen reader support, and block critical accessibility regressions.
