---
layout: default
meta_title: SUSTAINABILITY.md · SUSTAINABILITY.md
description: The open standard for sustainability transparency, governance, and lower-impact engineering workflows.
hero_title: SUSTAINABILITY.md
hero_lede_1: A practical, open format for documenting sustainability policy, governance, and engineering guardrails.
hero_lede_2: Think of SUSTAINABILITY.md as a <strong>README for digital sustainability</strong>: a predictable place for humans and AI coding agents to find your standards.
primary_cta_label: Explore Framework
primary_cta_url: "#framework"
secondary_cta_label: View on GitHub
secondary_cta_url: https://github.com/mgifford/sustainability.md
code_card_title: Simple Sample SUSTAINABILITY.md
code_card_link_label: See full starter policy
code_card_link_url: ./README.md
code_snippet: |
  # SUSTAINABILITY.md

  ## Team commitment
  - We will improve measurable impact every release
  - We treat sustainability like reliability and accessibility

  ## Accessibility as code
  - Run a11y checks in CI on pull requests
  - Block merges on new critical accessibility failures

  ## AI usage policy
  - Prefer deterministic alternatives first
  - Keep prompts minimal and disclose AI use in PRs

  ## Sustainability as code
  - Enforce page-weight and request budgets in CI
  - Require justification for third-party and AI-heavy additions
why_heading: Why SUSTAINABILITY.md?
framework_heading: The Framework
framework_cards:
  - title: Transparency & Disclosure
    body: Publish scope, baseline metrics, known gaps, and remediation plans with owners and dates.
  - title: Operational Governance
    body: Define labels, accountable owners, and merge criteria tied to sustainability thresholds.
  - title: Automation & Guardrails
    body: Enforce page-weight budgets, third-party review, media optimization, and regression tracking in CI.
examples_heading: Reference Examples
reference_cards:
  - title: Full Template
    label: SUSTAINABILITY-template.md
    url: ./SUSTAINABILITY-template.md
  - title: Action Playbook
    label: Team + AI implementation guide
    url: ./action-playbook/
  - title: Policy File
    label: README.md
    url: ./README.md
  - title: WSG Mapping
    label: WSG_REFERENCES.yaml
    url: ./WSG_REFERENCES.yaml
  - title: W3C WSG
    label: Web Sustainability Guidelines
    url: https://www.w3.org/TR/web-sustainability-guidelines/
  - title: WSG Resources
    label: Reference resources page
    url: ./resources/
  - title: Guidelines Data
    label: guidelines.json
    url: ./guidelines.json
  - title: Sustainable Web Design
    label: External companion resource
    url: ./sustainablewebdesign/
adopt_heading: How to Adopt
adopt_steps:
  - title: 1. Add SUSTAINABILITY.md
    body: Create it at your repository root and link it from README.
  - title: 2. Document what matters
    body: Include scope, metrics baselines, owners, and constraints for AI usage and third-party integrations.
  - title: 3. Enforce in CI
    body: Wire page-weight, request-count, and regression checks into pull requests.
  - title: 4. Keep it living
    body: Update policy and mappings as architecture, hosting, and tooling evolve.
footer_title: SUSTAINABILITY.md
footer_text: is an open policy format for digital sustainability transparency and governance.
---

README files are broad onboarding docs. SUSTAINABILITY.md adds an explicit
layer for environmental impact decisions, trade-offs, and operational controls.

**Status:** Draft (work in progress).

**AI disclosure:** This project has been developed with AI-assisted drafting
and implementation support, with human review and editing.

Keeping this guidance visible improves transparency, helps teams make
consistent choices, and gives AI coding agents clearer constraints by default.
