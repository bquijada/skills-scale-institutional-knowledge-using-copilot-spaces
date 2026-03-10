# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans ([Security Champion](octoacme-roles-and-personas.md#security-champion) sign-off)
- QA sign-off from [QA Lead](octoacme-roles-and-personas.md#qa-lead) confirming all release criteria verified
- Security Champion sign-off confirming no open critical/high vulnerabilities
- Operations readiness confirmation from [Operations Manager](octoacme-roles-and-personas.md#operations-manager) (infrastructure, runbooks, monitoring)
- UX review completed for user-facing changes ([UX Designer](octoacme-roles-and-personas.md#ux-designer))
- Customer Support briefed on changes, known issues, and FAQs ([Customer Support](octoacme-roles-and-personas.md#customer-support))
- Release notes drafted
- Rollback / mitigation plan documented

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — coordinated with [Operations Manager](octoacme-roles-and-personas.md#operations-manager)
- [ ] QA sign-off received ([QA Lead](octoacme-roles-and-personas.md#qa-lead))
- [ ] Security Champion sign-off received ([Security Champion](octoacme-roles-and-personas.md#security-champion))
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Operations Manager confirms staging environment healthy
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Operations Manager confirms production environment healthy
- [ ] Announce release to stakeholders and [Customer Support](octoacme-roles-and-personas.md#customer-support)

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - [Operations Manager](octoacme-roles-and-personas.md#operations-manager) triggers incident response and notifies on-call
  - Rollback to last known-good release if necessary
  - [Security Champion](octoacme-roles-and-personas.md#security-champion) reviews if security-related
  - [Customer Support](octoacme-roles-and-personas.md#customer-support) notified to communicate status to affected users
  - Triage root cause and capture action items
  - See [Escalation Paths](octoacme-risks-and-communication.md#escalation-paths) for full escalation guidance

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
