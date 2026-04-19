# Bug: Continue button behaves inconsistently after validation error

## Environment
- Platform: Android
- Device: Xiaomi Redmi Note 11
- OS: Android 11
- App version: HeroesSchool-v1.0-debug.apk

## Preconditions
User is on registration screen

## Description
- The "Continue" button behaves inconsistently depending on validation state.

- After entering invalid data and triggering a validation error, the button may remain active or behave incorrectly instead of reflecting validation status.

## Steps to Reproduce
1. Open registration screen
2. Enter invalid data in required field
3. Trigger validation error
4. Observe "Continue" button behavior

## Actual Result
The "Continue" button remains active or behaves inconsistently.

## Expected Result
The "Continue" button should be disabled when validation errors are present and enabled only when all required fields are valid.

## Severity
Medium

## Priority
Medium

## Frequency
Always

## Impact
May confuse users and lead to incorrect form submission behavior.

## Attachments:
<img width="399" height="823" alt="image" src="https://github.com/user-attachments/assets/80e3e19d-eb1a-4969-8db5-4ebe3b0688b3" />

## Notes
This issue suggests inconsistent validation logic between UI state and form validation rules.
