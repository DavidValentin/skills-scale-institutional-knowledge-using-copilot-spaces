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

## Definition of Ready & Done
- Issues must meet the **Definition of Ready** before entering the sprint (see [`octoacme-definition-of-ready-and-done.md`](octoacme-definition-of-ready-and-done.md)).
- Work is only marked **Done** when it meets the **Definition of Done**, including QA sign-off and documentation updates.

## QA Ownership & Handoffs
- **QA Lead** owns the QA column on the project board.
- A developer moves a ticket to **In Review** after opening a PR; once the PR is approved and merged it moves to **QA**.
- The QA Lead (or assigned tester) is responsible for verifying acceptance criteria in the QA column.
- If issues are found, the ticket is moved back to **In Progress** with a comment describing the failure.
- The QA Lead provides a written sign-off (comment or checklist) before a ticket moves to **Done**.
- For release readiness, the QA Lead reviews all QA-column and Done tickets and completes the [Release Readiness Checklist](octoacme-release-readiness-checklist.md).

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance: coordinated by the QA Lead
- Test coverage and defect metrics tracked and shared in sprint review

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
