# Bug: Profile update returns success but city value is not persisted

## Location
Profile → Edit Profile → City field

## Description
-When updating the city field with a value not from the predefined list, the system shows a success message.

-However, after reopening the profile, the city remains unchanged.

-This creates inconsistency between UI feedback and actual data persistence.

## Steps to Reproduce
1. Open Profile
2. Go to Edit Profile
3. Locate "City" field
4. Enter a custom city not from the suggested list
5. Tap "Save"
6. Reopen profile

## Actual Result
Success message is displayed, but city value remains unchanged.

## Expected Result
System should either:
- save the entered city correctly, OR
- restrict input to predefined values and prevent saving invalid input.

## Severity
Major

## Priority
Medium

## Frequency
Always

## Impact
Users may believe their data was updated successfully, leading to confusion and loss of trust.

## Notes
Possible backend validation silently rejects unsupported values.

## Environment:

- Device: Xiaomi Redmi Note 11
- OS: Android 11
- MIUI: 13.0.14
- Build: HeroesSchool-v1.0-debug.apk

## Additional information:

The same issue applies when choosing a child role.
