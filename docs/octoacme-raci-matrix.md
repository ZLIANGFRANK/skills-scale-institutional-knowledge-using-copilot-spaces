# OctoAcme — RACI Matrix and Contact Guide

## Purpose
Provide a quick-reference map of which role is **R**esponsible, **A**ccountable, **C**onsulted, or **I**nformed for key project activities. Use this to resolve uncertainty about ownership and to identify who to contact for each type of decision or handoff.

**RACI key:**
- **R** — Responsible: does the work
- **A** — Accountable: owns the outcome (one per activity)
- **C** — Consulted: provides input before or during the activity
- **I** — Informed: notified of progress or decisions

---

## RACI Matrix

| Activity | Developer | Technical Lead | QA Lead | Product Manager | Project Manager | Release Manager | Stakeholder Liaison | Compliance Officer |
|---|---|---|---|---|---|---|---|---|
| Define project goals & success metrics | C | C | I | **A/R** | C | I | C | I |
| Create and maintain backlog | C | C | C | **A/R** | C | I | C | I |
| Architectural design decisions | R | **A** | C | C | I | I | I | C |
| Sprint / iteration planning | R | C | C | C | **A** | I | I | I |
| Feature development | **A/R** | C | I | I | I | I | I | I |
| Code review | R | **A** | I | I | I | I | I | I |
| Define test strategy & acceptance criteria | C | C | **A/R** | C | I | I | I | I |
| Execute testing & acceptance sign-off | C | C | **A/R** | C | I | C | I | I |
| Risk identification & mitigation | C | C | C | C | **A** | C | C | C |
| Compliance review | I | C | C | C | C | C | I | **A/R** |
| Stakeholder communication & updates | I | I | I | C | C | I | **A/R** | I |
| Release planning & scheduling | C | C | C | C | C | **A/R** | I | I |
| Release readiness sign-off | C | C | R | C | C | **A** | I | R |
| Deploy to production | R | C | C | I | I | **A** | I | I |
| Post-deploy verification | R | C | R | I | I | **A** | I | I |
| Stakeholder release announcement | I | I | I | C | C | R | **A** | I |
| Incident response coordination | C | C | C | I | C | **A** | I | I |
| Retrospective facilitation | I | I | I | C | **A** | C | I | I |
| Continuous improvement tracking | C | C | C | C | **A** | C | I | I |

---

## Who to Contact Guide

Use the table below to quickly find the right person or role for common needs.

| If you need to… | Contact |
|---|---|
| Clarify a feature requirement or acceptance criteria | **Product Manager** |
| Understand technical design or architecture | **Technical Lead** |
| Report or triage a quality defect | **QA Lead** |
| Understand the release schedule or release status | **Release Manager** |
| Raise a stakeholder concern or get business context | **Stakeholder Liaison** |
| Report or resolve a compliance or policy question | **Compliance Officer** |
| Escalate a delivery risk or cross-team dependency | **Project Manager** |
| Get unblocked on a technical problem | **Technical Lead** or **Developers** |
| Request a change to project scope | **Product Manager** + **Project Manager** |

---

## Handoff Checklist: Sprint to Release

Use this checklist to verify a clean handoff from sprint completion to release readiness.

### Developer → QA Lead Handoff
- [ ] All acceptance criteria defined and attached to the issue/PR
- [ ] Feature branch merged to the integration branch
- [ ] Unit and integration tests passing in CI
- [ ] PR description includes testing notes and any known limitations
- [ ] Feature flagged off in production (if using feature flags)

### QA Lead → Release Manager Handoff
- [ ] Acceptance testing completed and sign-off documented
- [ ] All blocking defects resolved or deferred with Product Manager approval
- [ ] Test summary report shared with Release Manager and Project Manager
- [ ] Smoke test scripts updated for the new release

### Release Manager → Production Handoff
- [ ] Release notes drafted and reviewed by Product Manager
- [ ] Rollback plan documented and shared with the on-call team
- [ ] Compliance sign-off obtained (if required for the release)
- [ ] Deployment window confirmed with affected teams
- [ ] Stakeholder Liaison notified to prepare the release announcement

### Post-Release
- [ ] Post-deploy verification completed and results documented
- [ ] Stakeholder announcement published by Stakeholder Liaison
- [ ] Any production incidents captured in the risk register
- [ ] Retrospective scheduled by Project Manager

---

## Related Documents
- [Roles and Personas](octoacme-roles-and-personas.md)
- [Release and Deployment Guide](octoacme-release-and-deployment.md)
- [Risk Management and Communication](octoacme-risks-and-communication.md)
- [Execution and Tracking](octoacme-execution-and-tracking.md)
