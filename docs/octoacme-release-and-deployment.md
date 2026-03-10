# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared and executed by QA Lead
- QA Lead has completed the [Release Readiness Checklist](octoacme-release-readiness-checklist.md) and signed off
- Stakeholder Representative notified and has approved release window (for major/minor releases)
- DevOps/SRE has reviewed the deployment plan and confirmed environment readiness

## Change Management
- **Patch releases**: DevOps/SRE and Project Manager approve; team is notified via the release channel.
- **Minor releases**: Project Manager schedules deployment window; QA Lead and Stakeholder Representative sign off before deploy.
- **Major releases**: Full sign-off required from Project Manager, Product Manager, QA Lead, and Stakeholder Representative. Change ticket raised and approved in advance.
- All changes to production must be tracked in the release log with author, approver, and rollback plan.

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - Trigger incident response and notify on-call
  - Rollback to last known-good release if necessary
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
