# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI (coordinated by [Security Champion](octoacme-roles-and-personas.md#security-champion))
- Manual QA for feature acceptance when needed (led by [QA Lead](octoacme-roles-and-personas.md#qa-lead))
- Usability review for user-facing changes (led by [UX Designer](octoacme-roles-and-personas.md#ux-designer))
- Operational readiness check before release (led by [Operations Manager](octoacme-roles-and-personas.md#operations-manager))

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues
- Quality blocker: [QA Lead](octoacme-roles-and-personas.md#qa-lead) → Project Manager → Product Lead
- Security blocker: [Security Champion](octoacme-roles-and-personas.md#security-champion) → Security on-call → Project Manager
- Operational blocker: [Operations Manager](octoacme-roles-and-personas.md#operations-manager) → On-call team → Project Manager
- Customer-facing blocker: [Customer Support](octoacme-roles-and-personas.md#customer-support) → Project Manager → Operations Manager / Developers

> See [Escalation Paths](octoacme-risks-and-communication.md#escalation-paths) in the Risk Management & Communication doc for the full escalation matrix.

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Security scanning configured in CI ([Security Champion](octoacme-roles-and-personas.md#security-champion) responsible)
- [ ] QA test plan created and test cases documented ([QA Lead](octoacme-roles-and-personas.md#qa-lead) responsible)
- [ ] Operational runbooks and dashboards in place ([Operations Manager](octoacme-roles-and-personas.md#operations-manager) responsible)
- [ ] Design specs reviewed for usability and accessibility ([UX Designer](octoacme-roles-and-personas.md#ux-designer) responsible)
- [ ] Customer Support prepared with known issues and FAQ updates
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
