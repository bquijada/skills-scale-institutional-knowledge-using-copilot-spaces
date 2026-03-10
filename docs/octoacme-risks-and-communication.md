# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner (see [OctoAcme Personas](octoacme-roles-and-personas.md) for role definitions)
- Mitigation plan
- Status

**Owner role mapping:** Risk owners should be assigned to a named persona:
- Quality/testing risks → [QA Lead](octoacme-roles-and-personas.md#qa-lead)
- Security/compliance risks → [Security Champion](octoacme-roles-and-personas.md#security-champion)
- Infrastructure/deployment risks → [Operations Manager](octoacme-roles-and-personas.md#operations-manager)
- User experience risks → [UX Designer](octoacme-roles-and-personas.md#ux-designer)
- Customer impact risks → [Customer Support](octoacme-roles-and-personas.md#customer-support)

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication

### Stakeholder Groups
Identify all stakeholder groups and their communication needs:

| Stakeholder | Frequency | Channel | Owner |
|---|---|---|---|
| Engineering (Developers, QA Lead) | Daily standup + weekly sync | Project board, Slack | Project Manager |
| Security Champion | As-needed + per-release review | Email, meeting | Project Manager |
| Operations Manager | Weekly + pre/post release | Status report, meeting | Project Manager |
| Product Manager | Weekly alignment | Meeting, roadmap doc | Project Manager |
| UX Designer | Per sprint/milestone | Design review, Slack | Product Manager |
| Customer Support | Pre-release + incident | Release notes, email | Project Manager / Operations Manager |
| Executive Sponsors | Monthly | Status report | Project Manager |

### Communication Templates

**Weekly Status Template:**
- Progress this week:
- Next steps:
- Risks & blockers:
- QA/quality status:
- Security/operational notes:
- Ask / decisions needed:

**Pre-Release Stakeholder Notification:**
- Release name / version:
- Planned release date:
- Summary of changes:
- Known risks or caveats:
- QA sign-off status (QA Lead):
- Security review status (Security Champion):
- Operations readiness status (Operations Manager):
- Customer Support preparation notes:

**Incident Communication:**
- Triage summary
- Actions being taken
- Expected timeline
- Impact on customers (coordinated with Customer Support)
- Post-incident blameless retrospective scheduled

## Escalation Paths

| Level | Scenario | Escalation Path |
|---|---|---|
| 1 | Team-level blocker | Team triage in daily standup |
| 2 | Unresolved blocker | PM → Product Lead + dependent teams |
| 3 | Business-impacting issue | PM → Sponsor-level escalation |
| Quality | Release-blocking defect | QA Lead → Project Manager → Product Lead |
| Security | Security incident or vulnerability | Security Champion → Security on-call → Project Manager → Sponsor |
| Operations | Production incident or outage | Operations Manager → On-call team → Project Manager → Customer Support notification |
| UX | Usability blocker on critical flow | UX Designer → Product Manager → Project Manager |
| Support | Critical customer-facing issue | Customer Support → Project Manager → Operations Manager / Developers |

> For role definitions, see [OctoAcme Personas](octoacme-roles-and-personas.md).
