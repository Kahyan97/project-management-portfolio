# UAT Test Cases
## Corporate Back-Office Administration System

### Test Case Status

- Not Executed
- Pass
- Fail
- Blocked

---

## UAT-001 — User Login

**Related Requirement:** FR-001

**Related User Story:** US-001

**Priority:** High

### Preconditions

- Valid user account exists.
- User is authorized to access the system.
- UAT environment is available.

### Test Steps

1. Navigate to the login page.
2. Enter a valid username.
3. Enter a valid password.
4. Click Login.

### Expected Result

The user is successfully authenticated and redirected to the back-office dashboard.

**Expected Status:** Pass

---

## UAT-002 — Invalid Login

**Related Requirement:** FR-001

**Related User Story:** US-001

**Priority:** High

### Preconditions

- UAT environment is available.

### Test Steps

1. Navigate to the login page.
2. Enter an invalid username or password.
3. Click Login.

### Expected Result

The system rejects the login attempt and displays an appropriate error message.

**Expected Status:** Pass

---

## UAT-003 — Create Customer Record

**Related Requirement:** FR-003

**Related User Story:** US-003

**Priority:** High

### Preconditions

- Authorized back-office user is logged in.
- Required customer information is available.

### Test Steps

1. Navigate to Customer Management.
2. Select Create Customer.
3. Enter valid customer information.
4. Submit the form.

### Expected Result

The customer record is successfully created and a confirmation message is displayed.

**Expected Status:** Pass

---

## UAT-004 — Mandatory Field Validation

**Related Requirement:** FR-003

**Related User Story:** US-003

**Priority:** High

### Test Steps

1. Navigate to Create Customer.
2. Leave one or more mandatory fields blank.
3. Submit the form.

### Expected Result

The system prevents submission and displays appropriate validation messages.

**Expected Status:** Pass

---

## UAT-005 — Search Customer Record

**Related Requirement:** FR-003

**Related User Story:** US-004

**Priority:** High

### Preconditions

- Customer records exist.

### Test Steps

1. Navigate to Customer Management.
2. Enter valid search criteria.
3. Click Search.

### Expected Result

The system displays customer records matching the selected criteria.

**Expected Status:** Pass

---

## UAT-006 — Update Customer Record

**Related Requirement:** FR-003

**Related User Story:** US-005

**Priority:** Medium

### Preconditions

- Authorized user is logged in.
- Existing customer record is available.

### Test Steps

1. Search for an existing customer.
2. Open the customer record.
3. Modify an editable field.
4. Save the changes.

### Expected Result

The updated customer information is successfully saved and displayed.

**Expected Status:** Pass

---

## UAT-007 — View Operational Dashboard

**Related Requirement:** FR-004

**Related User Story:** US-006

**Priority:** High

### Preconditions

- Authorized user is logged in.
- Operational data is available.

### Test Steps

1. Navigate to the dashboard.
2. Review displayed operational information.
3. Apply available filters.

### Expected Result

The dashboard displays the expected operational information and applies filters correctly.

**Expected Status:** Pass

---

## UAT-008 — Generate Operational Report

**Related Requirement:** FR-005

**Related User Story:** US-007

**Priority:** High

### Preconditions

- Authorized reporting user is logged in.
- Reporting data is available.

### Test Steps

1. Navigate to Reporting.
2. Select a reporting period.
3. Generate the report.
4. Review the results.
5. Export the report.

### Expected Result

The system generates a report containing the correct records and allows the authorized user to export it successfully.

**Expected Status:** Pass

---

## UAT-009 — Unauthorized Reporting Access

**Related Requirement:** FR-005

**Related User Story:** US-007

**Priority:** High

### Preconditions

- User without reporting permission exists.

### Test Steps

1. Log in using a user without reporting access.
2. Attempt to access the Reporting module.

### Expected Result

The user is denied access to the reporting function.

**Expected Status:** Pass

---

## UAT-010 — View Audit Activity

**Related Requirement:** FR-006

**Related User Story:** US-008

**Priority:** Medium

### Preconditions

- Authorized administrator is logged in.
- System activity has been recorded.

### Test Steps

1. Navigate to Audit Activity.
2. Search for recent system activity.
3. Review the displayed information.

### Expected Result

The system displays the relevant user, date/time and activity information.

**Expected Status:** Pass
