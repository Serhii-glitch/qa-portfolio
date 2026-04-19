# Contact Form Checklist

## Scope
Testing contact form functionality, validation, UI, and user interactions.

---

## UI

- [ ] All required fields are displayed according to the design
- [ ] Field labels match the design (text, position, style)
- [ ] Placeholder text is displayed correctly in all applicable fields
- [ ] Phone number field follows expected behavior (no placeholder or correct placeholder as per design)
- [ ] Submit button is visible and properly styled
- [ ] UI elements are aligned correctly and do not overlap
- [ ] Form layout is responsive on different screen sizes

---

## Functional

- [ ] User can enter data into Name field
- [ ] User can enter data into Email field
- [ ] User can enter data into Message field
- [ ] User can submit form with valid data

---

## Validation

### Name

- [ ] Name field accepts valid input
- [ ] Name field does not accept empty value
- [ ] Name field enforces maximum length or shows validation error
- [ ] Name field correctly handles special characters (according to requirements)

### Email
- [ ] Email must be in valid format
- [ ] Invalid email shows error

### Message
- [ ] Message field requires minimum length
- [ ] Message field does not accept empty value

---

## Negative

- [ ] Form cannot be submitted with empty fields
- [ ] Form cannot be submitted with invalid email
- [ ] Error messages are displayed correctly

---

## Edge Cases

- [ ] Very long input is handled correctly
- [ ] Special characters are handled correctly

---

## Feedback

- [ ] Success message is displayed after submit
- [ ] Error message is shown when submission fails

---

## Notes

- Phone number field placeholder is missing → reported as a bug
