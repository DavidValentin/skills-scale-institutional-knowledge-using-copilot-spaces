# OctoAcme — Definition of Ready & Done

## Purpose
Shared criteria that the team uses to decide when work is ready to start (Definition of Ready) and when it is truly complete (Definition of Done). These checklists reduce ambiguity, improve handoffs, and prevent defects from slipping through.

---

## Definition of Ready (DoR)

An issue or user story is **Ready** to be pulled into a sprint when all of the following are true:

- [ ] A clear problem statement and user story are written (`As a <role>, I want <goal>, so that <benefit>`)
- [ ] Acceptance criteria are defined and agreed upon by the Product Manager, QA Lead, and at least one Developer
- [ ] UX designs or wireframes are attached (for user-facing features)
- [ ] Dependencies on other teams or issues are identified and unblocked (or a plan exists)
- [ ] The issue is estimated (story points or T-shirt size)
- [ ] Any compliance, security, or accessibility requirements are noted
- [ ] The issue is linked to the relevant epic or milestone

> **Owner**: Product Manager (with input from QA Lead and team)

---

## Definition of Done (DoD)

A ticket is **Done** and may be moved to the Done column only when all of the following are true:

### Code & Build
- [ ] All acceptance criteria are implemented and verified
- [ ] Code reviewed and approved by at least one peer
- [ ] All automated tests pass in CI (unit, integration, lint, security scan)
- [ ] No new critical or high-severity security findings introduced

### Quality
- [ ] QA Lead (or assigned tester) has verified acceptance criteria in the QA column
- [ ] Regression tests pass for affected areas
- [ ] Accessibility requirements verified (for user-facing changes)
- [ ] Known defects are either fixed or accepted and tracked as follow-up issues

### Documentation
- [ ] Inline code documentation updated where needed
- [ ] User-facing documentation updated (if feature changes visible behavior)
- [ ] Runbooks or deployment notes updated (if operational behavior changes)
- [ ] PR description links to the issue and summarizes the change

### Release
- [ ] Feature flag or rollout plan in place (if applicable)
- [ ] Release notes entry drafted
- [ ] Stakeholder Representative notified of changes that affect their area (if applicable)

> **Owner**: QA Lead confirms DoD before moving to Done; Project Manager is accountable for ensuring the process is followed.

---

## Tips
- Review DoR during backlog refinement to keep the backlog healthy.
- Include DoD as a PR checklist template so every contributor is reminded automatically.
- Revisit and update DoR/DoD at retrospectives based on team feedback.
