# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA Lead

### Role Summary
The QA Lead oversees the quality strategy for the project, coordinates testing plans, manages defect triage, and ensures release criteria are verified before any deployment.

### Responsibilities
- Define and maintain the overall quality strategy and test plans
- Coordinate manual and automated testing efforts across the team
- Lead defect triage and track resolution of quality issues
- Verify that acceptance criteria are met before sign-off
- Ensure regression coverage for critical flows
- Report quality metrics and trends to the Project Manager

### Goals
- Prevent regressions and defects from reaching production
- Reduce the cost of quality by shifting testing left
- Maintain clear, up-to-date test documentation and coverage reports

### Typical Communication
- Sprint planning and review sessions to validate acceptance criteria
- Defect triage meetings with Developers and Product Manager
- Pre-release sign-off reports shared with Project Manager and Operations Manager

### Interactions with Other Roles
- **Product Manager**: Clarifies acceptance criteria and expected behaviors for features
- **Developers**: Reviews implementation against test cases; aligns on testability requirements
- **Project Manager**: Reports quality status; flags release blockers and quality risks
- **Security Champion**: Coordinates security test cases and vulnerability validation
- **Operations Manager**: Aligns on operational readiness checks and smoke test coverage

---

## Security Champion

### Role Summary
The Security Champion advocates for secure design, reviews code and architecture for risks, and educates the team on security best practices to reduce vulnerabilities across the SDLC.

### Responsibilities
- Review code, architecture, and designs for security risks
- Maintain and update the security checklist for all releases
- Educate team members on secure coding practices and threat modeling
- Coordinate with Operations Manager on infrastructure security
- Ensure security scanning tools are configured and integrated in CI
- Track and escalate security findings in the Risk Register

### Goals
- Prevent security vulnerabilities from reaching production
- Embed security practices into the team's day-to-day workflow
- Ensure compliance with relevant security policies and standards

### Typical Communication
- Security review sessions during design and planning phases
- Security findings reports shared with Project Manager and Developers
- Post-incident security retrospectives and root cause reports

### Interactions with Other Roles
- **Project Manager**: Escalates security risks and tracks mitigation in the Risk Register
- **Developers**: Guides secure implementation; performs or coordinates code security reviews
- **QA Lead**: Defines and validates security-specific test cases
- **Operations Manager**: Coordinates on infrastructure hardening, access controls, and incident response
- **Product Manager**: Advises on security trade-offs in product decisions

---

## Operations Manager

### Role Summary
The Operations Manager manages infrastructure, supports deployment pipelines, ensures the reliability and scalability of systems, and coordinates incident response for production issues.

### Responsibilities
- Manage and maintain production and staging infrastructure
- Oversee deployment pipelines and release coordination
- Ensure system reliability, uptime, and scalability requirements are met
- Lead incident response and post-incident reviews
- Coordinate with Security Champion on infrastructure security
- Communicate post-release status and incidents to Customer Support and Project Manager

### Goals
- Maintain high availability and performance of production systems
- Reduce mean time to recovery (MTTR) for incidents
- Ensure smooth, low-risk deployment processes

### Typical Communication
- Pre-release deployment planning meetings with Project Manager and QA Lead
- Incident status updates shared with Project Manager and Customer Support
- Post-incident blameless retrospective reports

### Interactions with Other Roles
- **Project Manager**: Coordinates deployment windows and communicates operational risks
- **Developers**: Collaborates on deployment scripts, infrastructure needs, and observability
- **QA Lead**: Aligns on smoke tests and operational readiness checks post-deployment
- **Security Champion**: Partners on infrastructure security, access reviews, and incident response
- **Customer Support**: Provides timely status updates during and after incidents

---

## UX Designer

### Role Summary
The UX Designer creates user flows, wireframes, and prototypes to ensure solutions are user-centric and usable. They validate designs with users and ensure the product meets usability standards.

### Responsibilities
- Conduct user research and synthesize insights into design decisions
- Create wireframes, prototypes, and user flows for new features
- Partner with Product Manager to define and refine feature specifications
- Validate designs through usability testing and feedback sessions
- Ensure consistency with the design system and accessibility standards
- Participate in sprint reviews to gather feedback on delivered features

### Goals
- Deliver intuitive, accessible, and consistent user experiences
- Reduce usability issues discovered in QA or post-launch
- Increase user satisfaction and task completion rates

### Typical Communication
- Design reviews and critiques with Product Manager and Developers
- Usability test reports shared with Product Manager and Project Manager
- Design handoffs and annotated specs delivered to Developers

### Interactions with Other Roles
- **Product Manager**: Collaborates on feature definitions; translates business goals into user-centric designs
- **Developers**: Provides design handoffs; reviews implementations for fidelity to design intent
- **QA Lead**: Shares usability criteria and edge cases for test coverage
- **Customer Support**: Incorporates user feedback and support insights into design improvements
- **Project Manager**: Communicates design dependencies and timeline for design deliverables

---

## Customer Support

### Role Summary
Customer Support monitors user feedback and support channels, triages issues reported by end-users, and communicates product updates and resolutions to customers.

### Responsibilities
- Monitor and triage support tickets and user feedback channels
- Escalate critical bugs and issues to the Project Manager and Developers
- Communicate product updates, known issues, and resolutions to customers
- Document recurring issues to inform Product Manager prioritization
- Participate in release readiness reviews to prepare support content
- Coordinate with Operations Manager during and after incidents

### Goals
- Minimize customer impact from defects and incidents
- Provide timely, accurate, and empathetic communication to users
- Feed user insights back into the product and development process

### Typical Communication
- Regular syncs with Project Manager to stay informed on release schedules
- Incident status updates received from Operations Manager
- Support escalation reports delivered to Product Manager and Developers

### Interactions with Other Roles
- **Product Manager**: Shares user feedback and recurring issues to inform backlog prioritization
- **Project Manager**: Receives release schedules, status updates, and escalation resolutions
- **Operations Manager**: Coordinates during production incidents; receives status and ETA updates
- **Developers**: Escalates complex technical issues; receives resolution details for customer communication
- **QA Lead**: Provides real-world user issue patterns to enhance test coverage

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Cross-references to these personas can be found in:
  - [Project Management Overview](octoacme-project-management-overview.md) — Core Roles section
  - [Risk Management & Communication](octoacme-risks-and-communication.md) — Escalation Paths and Risk Register
  - [Execution & Tracking](octoacme-execution-and-tracking.md) — Quality & Testing and Escalation sections
  - [Release & Deployment](octoacme-release-and-deployment.md) — Pre-release requirements and Deployment Checklist
  - [Project Planning](octoacme-project-planning.md) — Planning Checklist

