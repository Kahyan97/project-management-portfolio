# API Testing
## Corporate Back-Office Administration System

### 1. Objective

API testing is performed to validate the behavior, response status and data structure of API endpoints used by the back-office system.

Testing is performed using Postman.

---

## 2. API Test Scope

The testing focuses on:

- HTTP response status
- Response structure
- Required fields
- Data availability
- Error handling
- Basic endpoint behavior

---

## 3. Test Environment

**Tool:** Postman

**API:** Public mock API

**Purpose:** Portfolio demonstration only

No production credentials, client information or proprietary APIs are used.

---

## 4. Test Cases

| Test ID | Scenario | Expected Result |
|---|---|---|
| API-001 | Retrieve valid customer | HTTP 200 and customer data returned |
| API-002 | Validate customer ID | Response contains customer ID |
| API-003 | Validate customer name | Response contains customer name |
| API-004 | Retrieve invalid customer | Appropriate error response returned |

---

## 5. Automated Assertions

The Postman collection contains automated assertions for:

- HTTP response status
- Customer ID presence
- Customer name presence
- Error response validation

---

## 6. Example Test

```javascript
pm.test("Response status is 200", function () {
    pm.response.to.have.status(200);
});
