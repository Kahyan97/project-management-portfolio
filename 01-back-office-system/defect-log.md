# Defect Log
## Corporate Back-Office Administration System

### 1. Purpose

The defect log records issues identified during System Testing and User Acceptance Testing.

Defects are tracked from identification through investigation, resolution, retesting and closure.

---

# 2. Defect Severity

| Severity | Description |
|---|---|
| Critical | Prevents core system operation or causes major business impact |
| High | Major functionality is unavailable or produces incorrect business results |
| Medium | Functionality is affected but a workaround may exist |
| Low | Minor issue with limited business impact |

---

# 3. Defect Priority

| Priority | Description |
|---|---|
| P1 | Immediate resolution required |
| P2 | High priority; resolve before release where possible |
| P3 | Normal priority |
| P4 | Low priority / future enhancement |

---

# 4. Defect Register

| ID | Related UAT | Defect | Severity | Priority | Owner | Status |
|---|---|---|---|---|---|---|
| DEF-001 | UAT-003 | Customer record cannot be saved when optional field is blank | Medium | P2 | Developer | Resolved |
| DEF-002 | UAT-008 | Report returns records outside the selected date range | High | P1 | Developer | Resolved |
| DEF-003 | UAT-009 | User without reporting permission can access reporting URL directly | High | P1 | Developer | Resolved |
| DEF-004 | UAT-010 | Audit timestamp displays incorrect timezone | Medium | P2 | Developer | Resolved |
| DEF-005 | UAT-007 | Dashboard filter does not refresh displayed data | Medium | P2 | Developer | Retest Required |

---

# 5. DEF-001 — Customer Record Validation

### Summary

Customer record cannot be saved when an optional field is left blank.

### Related UAT

UAT-003 — Create Customer Record

### Severity

Medium

### Priority

P2

### Steps to Reproduce

1. Log in as an authorized back-office user.
2. Navigate to Customer Management.
3. Select Create Customer.
4. Enter all required information.
5. Leave the optional field blank.
6. Click Save.

### Expected Result

The customer record should be successfully created because the field is optional.

### Actual Result

The system prevents the record from being saved.

### Impact

Users are unable to create certain valid customer records.

### Resolution

Validation logic was updated to correctly distinguish between mandatory and optional fields.

### Retest Result

Passed.

### Status

Closed.

---

# 6. DEF-002 — Incorrect Reporting Date Range

### Summary

Operational report includes records outside the selected reporting period.

### Related UAT

UAT-008 — Generate Operational Report

### Severity

High

### Priority

P1

### Steps to Reproduce

1. Log in as an authorized reporting user.
2. Navigate to Reporting.
3. Select a specific date range.
4. Generate the report.
5. Review the returned records.

### Expected Result

Only records within the selected date range should be displayed.

### Actual Result

The report includes records outside the selected date range.

### Impact

Business stakeholders may rely on inaccurate operational information.

### Resolution

The reporting query was updated to correctly apply the selected date boundaries.

### Retest Result

Passed.

### Status

Closed.

---

# 7. DEF-003 — Unauthorized Reporting Access

### Summary

A user without reporting permission can access the reporting module directly through the URL.

### Related UAT

UAT-009 — Unauthorized Reporting Access

### Severity

High

### Priority

P1

### Steps to Reproduce

1. Log in using a user without reporting permission.
2. Enter the reporting URL directly.
3. Attempt to access the reporting page.

### Expected Result

The user should be denied access.

### Actual Result

The reporting page is displayed.

### Impact

Unauthorized users may access restricted business information.

### Resolution

Server-side authorization validation was implemented for the reporting endpoint.

### Retest Result

Passed.

### Status

Closed.

---

# 8. DEF-004 — Incorrect Audit Timestamp

### Summary

Audit activity timestamps are displayed using an incorrect timezone.

### Related UAT

UAT-010 — View Audit Activity

### Severity

Medium

### Priority

P2

### Steps to Reproduce

1. Perform an administrative action.
2. Navigate to Audit Activity.
3. Review the recorded timestamp.

### Expected Result

The timestamp should reflect the agreed system timezone.

### Actual Result

The timestamp is displayed using a different timezone.

### Impact

Users may have difficulty determining the actual time an activity occurred.

### Resolution

Timezone configuration was standardized across the application and database.

### Retest Result

Passed.

### Status

Closed.

---

# 9. DEF-005 — Dashboard Filter

### Summary

Dashboard information does not refresh correctly when a filter is applied.

### Related UAT

UAT-007 — View Operational Dashboard

### Severity

Medium

### Priority

P2

### Steps to Reproduce

1. Log in as an authorized user.
2. Navigate to the dashboard.
3. Select a filter.
4. Apply the filter.
5. Review the displayed information.

### Expected Result

Dashboard information should refresh according to the selected filter.

### Actual Result

The dashboard continues displaying the previous dataset.

### Impact

Users may see outdated or misleading operational information.

### Resolution

Pending development validation.

### Retest Result

Pending.

### Status

Retest Required.

---

# 10. Defect Lifecycle

The project follows the following defect lifecycle:

```text
New
 ↓
Triaged
 ↓
Assigned
 ↓
In Progress
 ↓
Resolved
 ↓
Ready for Retest
 ↓
Retest
 ↓
 ┌───────────────┐
 │               │
 PASS           FAIL
 │               │
 ↓               └──→ Reopen
Closed
