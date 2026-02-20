# SUSTAINABILITY.md

> Template for teams that want a practical, measurable sustainability policy for engineering, accessibility, and AI usage.

## Status and ownership

- Status: Draft | Active | Archived
- Policy owner: [team or role]
- Last updated: [YYYY-MM-DD]
- Review cadence: [monthly/quarterly]

## Team commitment

We commit to reducing digital waste and emissions by making sustainability part
of normal delivery work. We optimize for measurable improvement over perfection,
and we treat sustainability as a quality attribute alongside reliability,
security, performance, and accessibility.

## Scope

This policy applies to:

- Repositories: [list]
- Products/services: [list]
- Build and deployment workflows: [list]
- Third-party services and scripts: [list]

Out of scope for now:

- [list known exclusions]

## Baseline metrics

| Metric | Baseline | Target | Owner | Check cadence |
| :--- | :--- | :--- | :--- | :--- |
| Core page weight | [value] | [value] | [owner] | [cadence] |
| Request count | [value] | [value] | [owner] | [cadence] |
| CI compute minutes | [value] | [value] | [owner] | [cadence] |
| Third-party scripts | [value] | [value] | [owner] | [cadence] |
| Accessibility violations (critical) | [value] | [value] | [owner] | [cadence] |
| AI calls per PR | [value] | [value] | [owner] | [cadence] |

## Pull request requirements

All pull requests should include:

- Expected sustainability impact (increase/decrease/no change)
- Accessibility impact summary
- Third-party impact summary
- AI assistance disclosure when used

PR template fields:

- Sustainability impact:
- Accessibility checks run:
- AI tools used (if any):

## Accessibility as code (required checks)

Minimum required CI checks for each pull request:

- Linting for accessibility rules in markup/components
- Automated accessibility testing for changed pages/components
- Keyboard and focus-state checks for interactive elements
- Color contrast checks for text and controls
- Regression gating on critical accessibility failures

Suggested workflow policy:

- Block merge when new critical accessibility violations are introduced.
- Allow temporary exceptions only with issue link, owner, and expiry date.

## Sustainability as code (required checks)

Minimum required CI checks for each pull request:

- Page-weight budget checks
- Request-count budget checks
- Third-party script inventory and diff checks
- Media optimization checks
- Build footprint checks (for example CI minutes or job count)

Suggested workflow policy:

- Block merge when budgets regress beyond agreed thresholds.
- Require explicit approval for threshold changes.

## AI usage policy

### Default behavior

- Prefer deterministic tools first.
- Use AI only when it materially reduces rework or delivery risk.
- Keep prompts small and task-scoped.

### Allowed uses

- Refactoring analysis
- Drafting and summarization where deterministic automation is unavailable
- Migration planning and triage

### Restricted uses

- No always-on AI generation in CI for routine tasks
- No large-context prompts for trivial formatting or deterministic transforms
- No AI calls when local tooling can produce equivalent output

### AI controls

- Limit model size and retries where practical
- Cache reusable outputs
- Track approximate AI call volume per issue/PR
- Review monthly and set reduction goals

## Time and space shifting

### Time shift

- Run deferrable jobs during lower-carbon windows where practical.
- Define maximum delay bounds for each job type.

### Space shift

- Prefer lower-carbon regions/providers when architecture allows.
- Use self-hosted runners for region-aware workloads when needed.

## Governance and exceptions

- Labels: `sustainability`, `accessibility`, `performance-budget`, `ai-usage`, `third-party-impact`
- Decision owners: [team]
- Exception process:
  1. Open issue with rationale
  2. Define owner and expiry date
  3. Add mitigation plan
  4. Revalidate before expiry

## References

- Web Sustainability Guidelines: https://www.w3.org/TR/web-sustainability-guidelines/
- Sustainable Web Design: https://sustainablewebdesign.org/
- Green Web Foundation CO2.js: https://github.com/thegreenwebfoundation/co2.js

## AI agent instruction block

Use in AGENTS.md, .cursorrules, or system prompts:

> Check SUSTAINABILITY.md before proposing or writing changes. Prefer low-compute deterministic solutions. Run required accessibility and sustainability checks in CI. If AI is used, keep context minimal, avoid duplicate calls, and disclose usage in the PR.
