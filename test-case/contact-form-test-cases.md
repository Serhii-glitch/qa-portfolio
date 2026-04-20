# Contact Form Test Cases

## Scope
Test cases covering core functionality, validation, and critical scenarios of the contact form.

---

### TC-01: Successful form submission

**Preconditions:**
- User is on Contact Form page

**Test Data:**
- Name: test tester 
- Email: test@example.com  
- Message: test

**Steps:**
1. Enter valid Name
2. Enter valid Email
3. Enter valid Message
4. Click "Submit"

**Expected Result:**
- Form is successfully submitted
- Success message is displayed
- Data is sent to the server
- Form fields are cleared

---

### TC-02: Submit form with empty fields

**Preconditions:**
- User is on Contact Form page

**Steps:**
1. Leave all fields empty
2. Click "Submit"

**Expected Result:**
- Validation errors are displayed for all required fields
- Form is not submitted

---

### TC-03: Invalid email format

**Preconditions:**
- User is on Contact Form page

**Test Data:**
- Email: testemail.com

**Steps:**
1. Enter valid Name
2. Enter invalid Email
3. Enter valid Message
4. Click "Submit"

**Expected Result:**
- Email validation error is displayed
- Form is not submitted

---

### TC-04: Email with leading and trailing spaces

**Preconditions:**
- User is on Contact Form page

**Test Data:**
- Email: "'space bar' test@example.com  'space bar'"

**Steps:**
1. Enter valid Name
2. Enter email with spaces
3. Enter valid Message
4. Click "Submit"

**Expected Result:**
- Spaces are trimmed OR validation error is displayed
- Behavior matches requirements
- Form submission follows validation rules

---

### TC-05: Name field validation (empty)

**Preconditions:**
- User is on Contact Form page

**Steps:**
1. Leave Name field empty
2. Fill other fields with valid data
3. Click "Submit"

**Expected Result:**
- Validation error for Name field is displayed
- Form is not submitted

---

### TC-06: Message field validation (empty)

**Preconditions:**
- User is on Contact Form page

**Steps:**
1. Leave Message field empty
2. Fill other fields with valid data
3. Click "Submit"

**Expected Result:**
- Validation error for Message field is displayed
- Form is not submitted

---

### TC-07: Very long message input

**Preconditions:**
- User is on Contact Form page

**Test Data:**
- Message: 1000+ characters

**Steps:**
1. Enter valid Name
2. Enter valid Email
3. Enter very long Message
4. Click "Submit"

**Expected Result:**
- Input is limited OR validation error is displayed
- Application does not crash
- UI remains stable

---

### TC-08: Double-click submit button

**Preconditions:**
- User is on Contact Form page

**Test Data:**
- Valid form data

**Steps:**
1. Fill all fields with valid data
2. Double-click "Submit"

**Expected Result:**
- Only one request is sent to the server
- No duplicate submissions are created
- UI behaves correctly

---

### TC-09: Script injection attempt

**Preconditions:**
- User is on Contact Form page

**Test Data:**
- Message: `<script>alert(1)</script>`

**Steps:**
1. Enter valid Name
2. Enter valid Email
3. Enter script into Message field
4. Click "Submit"

**Expected Result:**
- Script is not executed
- Input is treated as plain text or rejected
- Application remains secure

---

### TC-10: Network request validation

**Preconditions:**
- User is on Contact Form page
- DevTools (Network tab) is open

**Test Data:**
- Valid form data

**Steps:**
1. Fill all fields with valid data
2. Click "Submit"
3. Observe Network request

**Expected Result:**
- Request is sent to the server
- Request payload contains correct data
- Response status is successful
- Response is correctly processed by UI

---

### TC-11: Page refresh after submission

**Preconditions:**
- User is on Contact Form page

**Steps:**
1. Submit form with valid data
2. Refresh the page

**Expected Result:**
- Form is not resubmitted
- No duplicate request is sent
- Page loads in a correct state

---

### TC-12: Form behavior on slow internet connection

**Preconditions:**
- User is on Contact Form page
- Network throttling is enabled (Slow 3G or similar)

**Test Data:**
- Valid form data

**Steps:**
1. Fill all fields with valid data
2. Click "Submit"

**Expected Result:**
- Loading indicator is displayed
- UI does not freeze
- Request is completed successfully
- User receives feedback (success or error)
