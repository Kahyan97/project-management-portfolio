# Jira Project Backlog
## Corporate Back-Office Administration System

### 1. Overview

This backlog translates the approved business and functional requirements into actionable user stories for the development team.

The backlog is organized into Epics, User Stories, Acceptance Criteria, Priority, and Story Points.

---

# 2. Epics

| Epic | Description |
|---|---|
| EPIC-01 | User Authentication & Access Management |
| EPIC-02 | Customer Management |
| EPIC-03 | Operational Dashboard |
| EPIC-04 | Reporting |
| EPIC-05 | Audit & Activity Tracking |

---

# 3. User Stories

## EPIC-01 — User Authentication & Access Management

### US-001 — User Login

**User Story**

As a system user,  
I want to log into the back-office system using my credentials,  
so that I can securely access functions assigned to my role.

**Acceptance Criteria**

- User can enter username and password.
- System validates the credentials.
- Successful login redirects the user to the dashboard.
- Invalid credentials display an appropriate error message.
- Unauthorized users cannot access protected pages.

**Priority:** High

**Story Points:** 3

**Related Requirement:** FR-001

---

### US-002 — User Role Management

**User Story**

As an administrator,  
I want to assign roles to users,  
so that users only have access to functions relevant to their responsibilities.

**Acceptance Criteria**

- Administrator can create a user.
- Administrator can assign a role.
- Administrator can update a user's role.
- Administrator can deactivate a user.
- System applies the correct permissions based on the assigned role.

**Priority:** High

**Story Points:** 5

**Related Requirement:** FR-002

---

# EPIC-02 — Customer Management

### US-003 — Create Customer Record

**User Story**

As a back-office user,  
I want to create a customer record,  
so that customer information can be stored in the centralized system.

**Acceptance Criteria**

- User can enter required customer information.
- Mandatory fields are validated.
- System prevents duplicate records based on defined business rules.
- Successfully created records are stored in the database.
- User receives confirmation after successful creation.

**Priority:** High

**Story Points:** 5

**Related Requirement:** FR-003

---

### US-004 — Search Customer Records

**User Story**

As a back-office user,  
I want to search customer records,  
so that I can quickly locate the information I need.

**Acceptance Criteria**

- User can search using agreed search criteria.
- System displays matching records.
- No matching records display an appropriate message.
- Users can access customer details from the search results.

**Priority:** High

**Story Points:** 3

**Related Requirement:** FR-003

---

### US-005 — Update Customer Record

**User Story**

As a back-office user,  
I want to update customer information,  
so that records remain accurate and up to date.

**Acceptance Criteria**

- Authorized users can edit customer information.
- Mandatory fields are validated.
- Changes are saved successfully.
- Updated information is displayed after saving.
- Changes are recorded in the audit trail.

**Priority:** Medium

**Story Points:** 5

**Related Requirement:** FR-003

---

# EPIC-03 — Operational Dashboard

### US-006 — View Operational Dashboard

**User Story**

As a business stakeholder,  
I want to view key operational information on a dashboard,  
so that I can monitor business activities efficiently.

**Acceptance Criteria**

- Authorized users can access the dashboard.
- Dashboard displays agreed operational metrics.
- Data is retrieved from the latest available records.
- Users can apply available filters.
- Dashboard information is displayed clearly.

**Priority:** High

**Story Points:** 8

**Related Requirement:** FR-004

---

# EPIC-04 — Reporting

### US-007 — Generate Operational Report

**User Story**

As a business stakeholder,  
I want to generate operational reports,  
so that I can review and analyze business activities.

**Acceptance Criteria**

- User can select a reporting period.
- User can generate the report.
- Report contains records matching the selected criteria.
- User can export the report.
- Unauthorized users cannot access the reporting function.

**Priority:** High

**Story Points:** 5

**Related Requirement:** FR-005

---

# EPIC-05 — Audit & Activity Tracking

### US-008 — View Audit Activity

**User Story**

As an administrator,  
I want to view system activity logs,  
so that I can track important administrative actions.

**Acceptance Criteria**

- System records the user who performed an action.
- System records the date and time.
- System records the action performed.
- Authorized administrators can search and view audit records.

**Priority:** Medium

**Story Points:** 5

**Related Requirement:** FR-006

---

# 4. Initial Backlog Prioritization

| ID | User Story | Priority | Story Points | Status |
|---|---|---|---:|---|
| US-001 | User Login | High | 3 | To Do |
| US-002 | User Role Management | High | 5 | To Do |
| US-003 | Create Customer Record | High | 5 | To Do |
| US-004 | Search Customer Records | High | 3 | To Do |
| US-005 | Update Customer Record | Medium | 5 | To Do |
| US-006 | Operational Dashboard | High | 8 | To Do |
| US-007 | Generate Operational Report | High | 5 | To Do |
| US-008 | View Audit Activity | Medium | 5 | To Do |

---

# 5. Definition of Done

A user story is considered complete when:

- Requirements are understood and confirmed.
- Development has been completed.
- Code has been reviewed.
- Relevant testing has been completed.
- Critical defects have been resolved.
- Acceptance criteria have been satisfied.
- Business/UAT validation is completed where applicable.
- Documentation has been updated.
- The feature is ready for deployment.

---

# 6. Sprint Planning Assumption

The project will use two-week Agile sprints.

Initial sprint planning will prioritize foundational capabilities before advanced reporting and dashboard functionality.

Example sequencing:

### Sprint 1

- US-001 — User Login
- US-002 — User Role Management

### Sprint 2

- US-003 — Create Customer Record
- US-004 — Search Customer Records

### Sprint 3

- US-005 — Update Customer Record
- US-006 — Operational Dashboard

### Sprint 4

- US-007 — Generate Operational Report
- US-008 — View Audit Activity
