# OctoAcme — Release Readiness Checklist

## Purpose
A structured checklist to confirm that a release is safe to deploy. Complete this checklist before every minor or major release. For patches, use the abbreviated section at the end.

**Release:** `___________`  
**Release Type:** Patch / Minor / Major  
**Scheduled Date:** `___________`  
**Release Owner (Project Manager):** `___________`  
**QA Lead:** `___________`  
**DevOps/SRE:** `___________`

---

## 1. Scope & Requirements

- [ ] All planned issues/stories for this release are in the Done column
- [ ] Any descoped items are documented and tracked as follow-up
- [ ] Product Manager has confirmed scope is complete and meets release goals
- [ ] Stakeholder Representative has reviewed and accepted the release scope (minor/major)

## 2. Quality & Testing

- [ ] All automated tests pass (unit, integration, end-to-end) in CI
- [ ] Security scan completed with no new critical or high findings
- [ ] Manual QA completed for all user-facing changes (QA Lead sign-off)
- [ ] Regression tests executed for impacted areas
- [ ] Accessibility checks completed for user-facing changes
- [ ] Defect log reviewed; no open P0/P1 blockers remain
- [ ] QA Lead has signed off: `___________ (name/date)`

## 3. Documentation & Communication

- [ ] Release notes written and reviewed
- [ ] User-facing documentation updated (if applicable)
- [ ] Internal runbooks and deployment notes updated (if applicable)
- [ ] Support and operations teams briefed on changes
- [ ] Stakeholders notified of release date and key changes

## 4. Infrastructure & Deployment

- [ ] DevOps/SRE has reviewed and approved the deployment plan
- [ ] Staging deployment completed and smoke-tested successfully
- [ ] Deployment window confirmed (for planned outage or change window)
- [ ] Rollback plan documented and verified
- [ ] Feature flags configured correctly (if applicable)
- [ ] Monitoring and alerting confirmed active for the release

## 5. Change Management Approvals

- [ ] Project Manager approves release: `___________ (name/date)`
- [ ] QA Lead sign-off: `___________ (name/date)`
- [ ] DevOps/SRE sign-off: `___________ (name/date)`
- [ ] Product Manager sign-off (minor/major): `___________ (name/date)`
- [ ] Stakeholder Representative sign-off (major only): `___________ (name/date)`

---

## Patch Release Abbreviated Checklist

For hotfixes and critical patches only — skip sections above and use this shorter checklist:

- [ ] Root cause identified and fix verified locally and in CI
- [ ] QA Lead or senior developer has reviewed and approved the fix
- [ ] Rollback plan documented
- [ ] DevOps/SRE notified and ready to deploy
- [ ] Project Manager and on-call stakeholders informed
- [ ] Post-deploy verification completed

---

## Post-Release Verification

Complete within 1 hour of production deployment:

- [ ] Smoke tests pass in production
- [ ] No spike in error rates or latency on dashboards
- [ ] Key business flows verified manually (if applicable)
- [ ] Release announced to stakeholders and support channels
- [ ] Release log updated with deployment details

---

## References
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Definition of Ready & Done](octoacme-definition-of-ready-and-done.md)
- [Role RACI Matrix](octoacme-role-raci.md)
