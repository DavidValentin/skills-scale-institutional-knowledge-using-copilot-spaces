# OctoAcme — Role RACI Matrix

## Purpose
Maps key project activities to team roles using RACI (Responsible, Accountable, Consulted, Informed). Use this to resolve ambiguity about who does what and to identify gaps when onboarding new team members.

**Legend**
- **R** = Responsible (does the work)
- **A** = Accountable (owns the outcome, signs off)
- **C** = Consulted (input required before action)
- **I** = Informed (kept up to date)

---

## RACI Table

| Activity | Project Manager | Product Manager | Developer | QA Lead | DevOps / SRE | UX Designer | Stakeholder Rep | Documentation Specialist |
|---|---|---|---|---|---|---|---|---|
| Define project scope & milestones | A | C | C | I | I | I | C | I |
| Maintain project plan & timeline | R/A | I | I | I | I | I | I | I |
| Define product vision & roadmap | C | R/A | C | I | I | C | C | I |
| Write & prioritize backlog items | C | R/A | C | C | I | C | C | I |
| Define acceptance criteria | C | R/A | C | R | I | R | C | I |
| Definition of Ready sign-off | A | R | C | C | I | I | I | I |
| Technical design & architecture | I | C | R/A | C | C | I | I | I |
| Feature implementation | I | I | R/A | I | C | I | I | I |
| Code review | I | I | R | I | C | I | I | I |
| CI/CD pipeline & automation | C | I | C | C | R/A | I | I | I |
| UX design & prototyping | I | C | C | I | I | R/A | I | I |
| Usability / accessibility review | I | C | C | C | I | R/A | I | I |
| QA test planning | I | C | C | R/A | I | C | I | I |
| QA execution & sign-off | I | I | C | R/A | I | I | I | I |
| Definition of Done sign-off | A | I | C | R | I | I | I | C |
| Release readiness approval | R/A | C | I | C | C | I | C | I |
| Release / deployment | C | I | C | C | R/A | I | I | I |
| Change management approval | A | C | I | C | C | I | C | I |
| Incident response | C | I | C | I | R/A | I | I | I |
| Post-mortem & follow-up | A | C | C | C | R | I | I | R |
| Stakeholder status reporting | R/A | C | I | I | I | I | I | I |
| Risk management | R/A | C | C | C | C | I | C | I |
| Retrospective facilitation | R/A | C | C | C | C | C | C | I |
| Process documentation | C | C | C | C | C | C | I | R/A |
| Onboarding & knowledge transfer | C | C | C | C | C | C | I | R/A |

---

## Notes
- Where a cell shows **R/A**, the same person is both doing the work and accountable for the outcome.
- Adjust this matrix to reflect your team's actual staffing — on smaller teams one person may cover multiple roles.
- Review the RACI at project kickoff and update it when roles or responsibilities change.
- See [`octoacme-roles-and-personas.md`](octoacme-roles-and-personas.md) for full role descriptions.
