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

## Release Manager

### Role Summary
The Release Manager oversees the end-to-end release lifecycle, ensuring that software versions are delivered on schedule, meet quality gates, and can be safely rolled back if needed. They act as the coordination hub between engineering, QA, and operations during every release cycle.

### Responsibilities
- Own and maintain the release calendar and release plan
- Coordinate release readiness reviews across engineering, QA, and operations
- Verify all acceptance criteria, CI gates, and security scans are passing before promotion
- Draft and publish release notes and communicate release status to stakeholders
- Own the rollback plan and coordinate incident response for failed deployments
- Track and report release metrics (release frequency, lead time, change failure rate)

### Goals
- Ship high-quality releases on a predictable, low-risk cadence
- Minimize production incidents caused by poorly coordinated releases
- Continuously improve the release pipeline and deployment process

### Typical Communication
- Pre-release readiness meetings with QA Lead, Technical Lead, and Project Manager
- Release announcements to stakeholders and support teams
- Post-release retrospectives and incident reports

### How They Interact With Existing Roles
- **Developers:** Reviews merged PRs for release eligibility; coordinates feature freeze and code-cut dates
- **Product Managers:** Aligns release scope and timing with roadmap milestones
- **Project Managers:** Syncs on schedule, risks, and escalation points; updates the risk register for release-related risks

---

## Stakeholder Liaison

### Role Summary
The Stakeholder Liaison is the primary bridge between external or internal stakeholders and the delivery team. They gather requirements and feedback, translate business needs into actionable inputs, and ensure stakeholders are informed of project progress.

### Responsibilities
- Identify and maintain the stakeholder registry (who needs what information and when)
- Gather business requirements, feedback, and approval decisions from stakeholder groups
- Represent stakeholder interests in planning and review meetings
- Communicate project status, decisions, and trade-offs back to stakeholders in accessible language
- Escalate unresolved stakeholder concerns to the Project Manager or Product Manager

### Goals
- Ensure stakeholder expectations are understood, managed, and met
- Reduce miscommunication and late-breaking requirement changes
- Build trust between the delivery team and business stakeholders

### Typical Communication
- Regular stakeholder briefings (weekly or milestone-based)
- Requirements and feedback summaries shared with the Product Manager
- Escalation memos for unresolved issues or conflicting priorities

### How They Interact With Existing Roles
- **Developers:** Provides clarification on business context and acceptance criteria during development
- **Product Managers:** Delivers stakeholder requirements and feedback to inform backlog prioritization
- **Project Managers:** Coordinates communication plans and escalation paths; co-owns stakeholder updates

---

## Compliance Officer

### Role Summary
The Compliance Officer ensures that the project adheres to applicable organizational policies, regulatory requirements, and security standards throughout the project lifecycle. They guide the team on compliance obligations and verify that required documentation and controls are in place before release.

### Responsibilities
- Identify and document applicable compliance requirements (e.g., data privacy, security, audit)
- Review project artifacts (design docs, data flows, release notes) for compliance gaps
- Guide the team on how to meet regulatory obligations without blocking delivery
- Verify compliance checkpoints are satisfied in release readiness reviews
- Maintain a compliance log and communicate open findings to the Project Manager

### Goals
- Protect the organization from regulatory and reputational risk
- Embed compliance checks into the delivery process rather than treating them as a last-minute gate
- Ensure all releases include required documentation and evidence for audit purposes

### Typical Communication
- Compliance reviews during planning, design, and pre-release phases
- Written findings reports shared with the Project Manager and Product Manager
- Training or guidance sessions for the team on new or changing requirements

### How They Interact With Existing Roles
- **Developers:** Reviews technical designs and data handling approaches; flags requirements early to avoid rework
- **Product Managers:** Ensures product features align with policy and regulatory constraints
- **Project Managers:** Provides compliance status updates for the risk register and escalates blockers

---

## QA Lead / Test Lead

### Role Summary
The QA Lead defines and owns the overall quality strategy for the project. They coordinate testing activities across the team, ensure test coverage aligns with acceptance criteria, and act as the final quality gate before release.

### Responsibilities
- Define the test strategy, test plan, and Definition of Done quality criteria
- Coordinate unit, integration, and end-to-end test efforts across the delivery team
- Maintain the QA environment and test data infrastructure
- Execute or oversee final acceptance testing before each release
- Report quality metrics (test coverage, defect rates, escape rate) to the Project Manager

### Goals
- Ensure every release meets the agreed quality bar
- Catch defects as early as possible to reduce the cost of rework
- Foster a team-wide culture of quality and continuous testing

### Typical Communication
- Daily coordination with Developers on test coverage and defect resolution
- Pre-release sign-off communication to the Release Manager and Project Manager
- QA status reports at sprint demos and release readiness reviews

### How They Interact With Existing Roles
- **Developers:** Partners on test design, reviews acceptance criteria, and co-owns the Definition of Done
- **Product Managers:** Validates that acceptance criteria are testable and complete
- **Project Managers:** Reports quality status and flags risks that may affect the release schedule

---

## Technical Lead / Architect

### Role Summary
The Technical Lead guides the technical direction of the project. They make or facilitate architectural decisions, ensure engineering best practices are followed, and serve as a technical escalation point for the development team.

### Responsibilities
- Define and maintain the technical architecture and key design decisions
- Review high-impact pull requests and technical design documents
- Identify and mitigate technical risks (e.g., scalability, security, maintainability)
- Mentor developers and raise the technical quality bar across the team
- Collaborate with the Product Manager on technical trade-offs and feasibility

### Goals
- Deliver a solution that is scalable, secure, and maintainable long-term
- Reduce technical debt and unplanned rework
- Enable the team to work effectively through clear technical standards and guidance

### Typical Communication
- Architecture decision records (ADRs) and design documents
- Code review feedback and technical guidance in PR comments
- Technical risk updates in weekly delivery syncs

### How They Interact With Existing Roles
- **Developers:** Provides technical direction, mentorship, and code review oversight
- **Product Managers:** Advises on technical feasibility and surfaces trade-offs for prioritization decisions
- **Project Managers:** Reports technical risks and estimates; flags architecture decisions that affect scope or timeline

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [RACI Matrix and Contact Guide](octoacme-raci-matrix.md) for a summary of which persona is responsible for each key activity.

