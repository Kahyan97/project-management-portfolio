# Risk Register
## Corporate Back-Office Administration System

### 1. Purpose

The risk register identifies potential events that may affect project scope, schedule, quality, or delivery.

Risks are assessed based on their probability and potential impact. Mitigation actions are defined to reduce the likelihood or impact of identified risks.

---

# 2. Risk Scoring Method

## Probability

| Score | Probability |
|---:|---|
| 1 | Very Low |
| 2 | Low |
| 3 | Medium |
| 4 | High |
| 5 | Very High |

## Impact

| Score | Impact |
|---:|---|
| 1 | Very Low |
| 2 | Low |
| 3 | Medium |
| 4 | High |
| 5 | Very High |

### Risk Score

Risk Score = Probability × Impact

| Score | Risk Level |
|---:|---|
| 1–4 | Low |
| 5–9 | Medium |
| 10–16 | High |
| 17–25 | Critical |

---

# 3. Risk Register

| ID | Risk | Probability | Impact | Score | Level | Owner | Mitigation | Status |
|---|---|---:|---:|---:|---|---|---|---|
| R-001 | Requirements change during development | 4 | 4 | 16 | High | Project Manager | Establish change control and assess impact before approval | Open |
| R-002 | Development activities fall behind schedule | 3 | 4 | 12 | High | Project Manager | Monitor sprint progress and blockers daily | Open |
| R-003 | Business stakeholders unavailable for UAT | 3 | 5 | 15 | High | PM Analyst | Confirm UAT schedule early and obtain stakeholder commitment | Open |
| R-004 | API integration issues delay testing | 3 | 5 | 15 | High | System Analyst | Conduct early API validation and integration testing | Open |
| R-005 | Production deployment failure | 2 | 5 | 10 | High | Technical Lead | Prepare deployment checklist, smoke tests and rollback plan | Open |
| R-006 | High-priority defects remain before UAT | 3 | 4 | 12 | High | QA Lead | Track defect trends and prioritize critical defects | Open |
| R-007 | External vendor delays | 3 | 4 | 12 | High | Project Manager | Establish vendor milestones and escalation process | Open |
| R-008 | Stakeholders have different expectations | 3 | 4 | 12 | High | Project Manager | Conduct regular alignment meetings and document decisions | Open |

---

# 4. Risk Response Strategy

## R-001 — Requirements Change

### Risk

Business requirements may change after development has started.

### Potential Impact

- Development rework
- Sprint disruption
- Increased project timeline
- Additional testing effort

### Mitigation

- Establish a formal change request process.
- Assess scope, timeline, resource and technical impact.
- Obtain appropriate approval before implementing significant changes.
- Maintain requirements traceability.

### Trigger

A stakeholder requests a change to an approved requirement.

---

## R-002 — Development Delay

### Risk

Development tasks may not be completed within the planned sprint.

### Potential Impact

- Sprint objectives not achieved
- Subsequent activities delayed
- UAT timeline affected

### Mitigation

- Monitor Jira progress regularly.
- Discuss blockers during Daily Scrum.
- Identify dependencies early.
- Escalate critical blockers promptly.
- Re-prioritize backlog items where appropriate.

### Trigger

A critical task is approaching its deadline without sufficient progress.

---

## R-003 — UAT Stakeholder Availability

### Risk

Business stakeholders may not be available during the planned UAT period.

### Potential Impact

- UAT delay
- Deployment delay
- Reduced confidence in business readiness

### Mitigation

- Confirm stakeholder availability before UAT begins.
- Schedule UAT sessions in advance.
- Provide test scenarios early.
- Assign backup business representatives where possible.

### Trigger

Stakeholder informs the project team that they cannot participate in scheduled UAT.

---

## R-004 — API Integration Issues

### Risk

API integration may fail or behave differently between environments.

### Potential Impact

- Integration testing failure
- Data inconsistencies
- Development rework
- UAT delay

### Mitigation

- Validate API endpoints early.
- Use Postman for API testing.
- Confirm request and response specifications.
- Test error handling.
- Maintain API test results.

### Trigger

API response does not match the agreed specification.

---

## R-005 — Production Deployment Failure

### Risk

Production deployment may fail because of configuration, infrastructure or application issues.

### Potential Impact

- Service disruption
- Delayed release
- Business impact

### Mitigation

- Prepare deployment checklist.
- Confirm production readiness.
- Conduct pre-deployment validation.
- Prepare rollback procedure.
- Conduct post-deployment smoke testing.

### Trigger

Deployment validation fails or critical functionality is unavailable after deployment.

---

# 5. Risk Monitoring

Risks will be reviewed during weekly project status meetings.

Risk monitoring activities include:

- Reviewing risk status.
- Identifying new risks.
- Updating probability and impact.
- Tracking mitigation actions.
- Escalating high and critical risks.
- Closing risks that are no longer applicable.

---

# 6. Escalation Criteria

Risks should be escalated when:

- Risk score reaches Critical level.
- Risk threatens a major project milestone.
- Risk affects production deployment.
- Risk requires management approval.
- Mitigation actions cannot be completed by the assigned owner.
- Risk impact exceeds the project team's authority to resolve.

---

# 7. Risk Review Frequency

| Activity | Frequency |
|---|---|
| Project team risk review | Weekly |
| High-risk review | Weekly |
| Critical-risk escalation | Immediate |
| Risk register update | As required |
| Project risk review | At major milestones |
