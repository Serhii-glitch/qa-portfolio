# Contact Form Checklist

## Scope
Testing contact form functionality including UI, validation, submission, edge cases, security, and network behavior.

---

## UI

- [ ] All required fields are displayed according to the design
- [ ] Field labels match the design (text, position, style)
- [ ] Placeholder text is displayed correctly
- [ ] Phone number field has correct placeholder behavior
- [ ] Submit button is visible and properly styled
- [ ] UI elements are aligned correctly and do not overlap
- [ ] Form layout is responsive on different screen sizes

---

## Functional

- [ ] User can enter data into Name field
- [ ] User can enter data into Email field
- [ ] User can enter data into Message field
- [ ] Form can be submitted with valid data
- [ ] Form allows repeated submissions after success

---

## Validation

### Name

- [ ] Name field accepts valid input
- [ ] Name field does not accept empty value
- [ ] Name field enforces minimum length requirement
- [ ] Name field enforces maximum length or shows validation error
- [ ] Name field correctly handles special characters (according to requirements)

### Email

- [ ] Email field accepts valid email format
- [ ] Email field requires "@" symbol
- [ ] Email field requires domain part
- [ ] Email field does not accept spaces
- [ ] Invalid email formats trigger validation error
- [ ] Email field trims leading and trailing spaces

### Message

- [ ] Message field accepts valid input
- [ ] Message field does not accept empty value
- [ ] Message field enforces minimum length requirement
- [ ] Message field enforces maximum length or shows validation error

---

## Negative

- [ ] Form cannot be submitted with empty fields
- [ ] Form cannot be submitted with invalid email
- [ ] Validation errors are displayed correctly
- [ ] Multiple rapid submissions do not create duplicate requests

---

## Edge Cases

- [ ] Message field accepts or properly validates emoji input
- [ ] Message field handles very long input (e.g., 1000+ characters)
- [ ] Email field trims leading spaces
- [ ] Email field trims trailing spaces or shows validation error
- [ ] Double-clicking submit does not send multiple requests
- [ ] HTML tags are not executed and are displayed safely
- [ ] Page refresh after submission does not resubmit data
- [ ] Browser autofill works correctly
- [ ] Form behaves correctly on slow internet connection (loading indicator, no UI freeze)

---

## Feedback

- [ ] Success message is displayed after successful submission
- [ ] Error message is displayed when submission fails
- [ ] Form fields are cleared after successful submission

---

## Security

- [ ] Script injection (`<script>alert(1)</script>`) is not executed
- [ ] SQL injection input is not executed
- [ ] Application safely handles malicious input
- [ ] Sensitive data is not exposed in UI or responses
- [ ] Data is transmitted over HTTPS

---

## Console / Network

- [ ] No errors appear in browser console during form interaction
- [ ] Network request is sent on form submission
- [ ] Request payload contains correct data
- [ ] Server returns successful response (e.g., 200 status)
- [ ] Response is correctly handled by the UI

---

## Notes

- Phone number field placeholder is missing → reported as a bug
