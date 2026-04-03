# OctoAcme Project Management Docs

This README provides an overview of the project management processes used by OctoAcme, with direct links to each process document in this folder.

## Docs List

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution and Tracking](octoacme-execution-and-tracking.md)
- [Risks and Communication](octoacme-risks-and-communication.md)
- [Release and Deployment](octoacme-release-and-deployment.md)
- [Retrospective and Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](octoacme-roles-and-personas.md)

## Process Summary

OctoAcme uses a lightweight, iterative project management lifecycle designed for cross-functional delivery, anchored by clear ownership and a consistent set of artifacts. Work flows through five phases—**initiation**, **planning**, **execution & tracking**, **release & deployment**, and **close & retrospective/continuous improvement**—guided by principles such as customer-first delivery, small testable increments, data-informed decisions, and psychological safety. Core artifacts include a project charter/one-pager, roadmap and release plan, sprint/iteration backlog, explicit acceptance criteria and a Definition of Done, a risk register, and retrospective action items.

Day-to-day execution is organized on a project board (Backlog → Ready → In Progress → In Review → QA → Done) and reinforced by PR practices: small PRs when possible, acceptance criteria linked in the PR description, CI checks for tests and lint, and required approvals before merge. Releases follow a standardized pre-release checklist (acceptance criteria met, CI/security scans passing, release notes, rollback plan, smoke tests) and a staged deployment process with post-deploy verification, stakeholder announcements, and blameless retrospectives that feed concrete, owned improvement items back into the backlog.

## Roles

| Role | Responsibilities |
|------|-----------------|
| **Project Manager (PM)** | Coordinates schedules, delivery execution, risks/dependencies, meeting facilitation, and status reporting. |
| **Product Manager / Product Lead (PdM)** | Defines outcomes, success metrics, and backlog prioritization. |
| **Developers** | Design, build, and test features; participate in reviews, estimation, and technical risk mitigation. |
| **QA / Testing** | Validates quality against acceptance criteria and the Definition of Done. |
| **Stakeholders** | Provide input, approvals, and business context. |

## Communication & Cadence

- **Weekly PM ↔ Product Lead alignment** – keep roadmap, priorities, and risks in sync.
- **Daily (or as agreed) standups** – delivery team progress and blockers.
- **Weekly delivery sync** – progress review, risk register update, dependency check.
- **Sprint / milestone demos** – demonstrate completed work to stakeholders.
- **Monthly / milestone stakeholder updates** – formal status, metrics, and decisions.
- **Single source of truth** – all status, decisions, and artifacts kept current in the project repository.
- **Risk register review & escalation path** – team → PM → Product Lead → sponsor, with explicit guidance for incident and security-incident communication.

## Quality & Release Practices

- **Testing:** unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows, and security scanning in CI.
- **Manual QA:** performed as needed before release.
- **Pre-release gates:** acceptance criteria met, CI and security scans passing, release notes written, rollback plan documented, smoke tests ready.
- **Deployment:** staged rollout (staging → production) with post-deploy verification and stakeholder announcement.
- **Retrospectives:** blameless review after each release; action items are owned, tracked, and fed back into the backlog for continuous improvement.
