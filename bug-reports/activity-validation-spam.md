# Bug: Validation error message repeatedly appears after entering invalid activity input

## Location
Profile → Edit Profile → Activity field

## Description
- When entering less than the required number of characters in the "Activity" field, a validation error message appears.

- However, the error message continues to appear repeatedly even after correcting the input and entering a valid value.

- The issue persists for several seconds even after valid input is entered and the "Save" button is pressed.

## Steps to Reproduce
1. Open profile edit screen
2. Go to "Activity" field
3. Enter less than 5 characters
4. Observe validation error message
5. Enter valid input (5+ characters)
6. Tap "Save"
7. Observe behavior

## Actual Result
Validation error message continues to appear repeatedly even after valid input is entered and saved.

## Expected Result
Validation error message should disappear immediately after valid input is entered.

## Severity
Major

## Priority
Medium

## Frequency
Always

## Impact
Creates poor user experience and may confuse users by displaying incorrect validation state.

## Environment:
- Device: Xiaomi Redmi Note 11
- OS: Android 11
- MIUI: 13.0.14
- Build: HeroesSchool-v1.0-debug (1).apk

## Attachments:


https://github.com/user-attachments/assets/352f5d48-8877-43e5-a1f0-6569e78f74d5

## Notes
Possible issue with validation state not being reset properly or multiple validation triggers without debounce.

