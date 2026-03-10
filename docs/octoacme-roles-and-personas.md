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
The QA Lead owns the overall test strategy, ensures quality gates are met before releases, and coordinates testing activities across the team.

### Responsibilities
- Define and maintain the test strategy (unit, integration, end-to-end, regression)
- Write and review acceptance criteria and Definition of Done
- Coordinate manual and automated QA activities
- Manage the QA column on the project board and track test outcomes
- Sign off on release readiness from a quality perspective
- Report defects and track resolution with developers

### Goals
- Prevent defects from reaching production
- Shorten feedback loops by integrating testing early in the cycle
- Ensure every release meets agreed quality standards

### Typical Communication
- Sprint planning and backlog refinement (reviewing acceptance criteria)
- Daily standups (flagging blocked QA items)
- QA sign-off reports before each release
- Post-release defect summaries and retrospective inputs

### Interactions with Existing Roles
- **Project Manager**: Reports QA status and risks; coordinates release readiness sign-off.
- **Product Manager**: Collaborates on acceptance criteria and priority of defect fixes.
- **Developers**: Reviews PRs for testability; pairs on reproducing and fixing defects; unblocks QA column items.

---

## DevOps / Site Reliability Engineer (SRE)

### Role Summary
The DevOps/SRE role owns the reliability, deployment automation, and operational health of the product. They build and maintain CI/CD pipelines, manage environments, and support incident response.

### Responsibilities
- Design and maintain CI/CD pipelines and deployment automation
- Manage staging and production environment configuration
- Define and enforce infrastructure-as-code and security scanning standards
- Support the team during deployments and own rollback procedures
- Monitor system health (latency, error rate, availability) and own alerting
- Lead incident response and post-mortems for production issues

### Goals
- Achieve fast, safe, and repeatable deployments
- Maintain high availability and performance targets
- Reduce toil through automation

### Typical Communication
- Sprint planning (estimating infrastructure and tooling work)
- Deployment runbooks and change management documentation
- On-call rotation and incident channels
- Post-mortem write-ups

### Interactions with Existing Roles
- **Project Manager**: Coordinates deployment windows, communicates environment risks and outages.
- **Product Manager**: Provides input on reliability requirements and non-functional acceptance criteria.
- **Developers**: Reviews code for deployability and security; pairs on CI configuration and environment issues.
- **QA Lead**: Ensures staging environments match production for reliable QA outcomes.

---

## UX Designer

### Role Summary
The UX Designer creates user-centered designs that ensure features are intuitive, accessible, and aligned with user needs. They translate requirements into wireframes, prototypes, and design specifications.

### Responsibilities
- Conduct user research and usability testing
- Produce wireframes, interaction flows, and high-fidelity prototypes
- Define and maintain the design system and component library
- Collaborate on acceptance criteria to include usability and accessibility standards
- Review implemented features for design fidelity

### Goals
- Deliver experiences that are usable, accessible, and delightful
- Reduce re-work by resolving design ambiguity before development begins
- Advocate for the end user throughout the product lifecycle

### Typical Communication
- Discovery and planning sessions with Product Manager
- Design review meetings and prototype walkthroughs with developers
- Usability test reports shared with Product Manager and stakeholders

### Interactions with Existing Roles
- **Project Manager**: Aligns design milestones with the project schedule; flags scope creep in design deliverables.
- **Product Manager**: Co-defines user stories and acceptance criteria; validates designs against product goals.
- **Developers**: Provides annotated designs and answers implementation questions; reviews UI PRs for fidelity.
- **QA Lead**: Shares design specs so QA can validate visual and interaction correctness.

---

## Stakeholder Representative

### Role Summary
The Stakeholder Representative acts as the primary liaison between external or senior stakeholders and the delivery team. They surface business requirements, validate priorities, and communicate project status upward.

### Responsibilities
- Represent stakeholder interests and business requirements in planning sessions
- Review and approve high-level feature prioritization and scope changes
- Flag business risks, compliance requirements, and strategic dependencies early
- Ensure stakeholder feedback is captured and incorporated into the backlog
- Communicate project status and milestone achievements to the broader organization

### Goals
- Keep stakeholder expectations aligned with delivery realities
- Ensure business value is maximized and risks are visible
- Reduce last-minute scope changes through early engagement

### Typical Communication
- Sprint review / demo attendance and feedback
- Bi-weekly or monthly steering updates with Project Manager
- Issue and risk escalation as needed

### Interactions with Existing Roles
- **Project Manager**: Key partner for status reporting, risk escalation, and scope change approval.
- **Product Manager**: Provides business context and validates roadmap priorities against strategic goals.
- **Developers**: Participates in demos to give direct feedback on delivered features.
- **QA Lead**: Reviews release readiness reports before approving production rollouts.

---

## Documentation Specialist

### Role Summary
The Documentation Specialist ensures that process artifacts, technical guides, and runbooks are accurate, accessible, and up to date. They support onboarding and knowledge transfer across the team.

### Responsibilities
- Maintain and improve process documentation (this document set)
- Collaborate with engineers to produce and review technical runbooks and ADRs
- Ensure new features and process changes are reflected in documentation before release
- Own the documentation review checklist in the Definition of Done
- Support onboarding by keeping getting-started guides current

### Goals
- Reduce knowledge silos and ramp-up time for new team members
- Ensure documentation is always in sync with the current state of the product and process
- Make institutional knowledge discoverable and reusable

### Typical Communication
- Documentation review comments in PRs
- Bi-weekly documentation sync with PM and tech leads
- Documentation status updates in sprint reviews

### Interactions with Existing Roles
- **Project Manager**: Aligns on which documentation is required per milestone; flags documentation debt.
- **Product Manager**: Translates feature specs and user research findings into user-facing documentation.
- **Developers**: Reviews technical docs for accuracy; requests runbooks and ADRs as part of the Definition of Done.
- **QA Lead**: Ensures test plans and QA processes are documented and version-controlled.
- **DevOps/SRE**: Collaborates on deployment runbooks and incident response playbooks.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [`octoacme-role-raci.md`](octoacme-role-raci.md) for a RACI matrix mapping roles to key project activities.

