# Bug: App crashes when selecting "Speaker" role and uploading profile photo during registration

## Preconditions
User is on registration flow

## Description
-The application crashes during registration when selecting the "Speaker" role and uploading a profile photo.

-The issue does not occur when selecting other roles (e.g., "Child"), where the flow works correctly.

## Steps to Reproduce
1. Open the app
2. Start registration process
3. Complete initial steps
4. Select "Speaker" role
5. Proceed to photo upload step
6. Upload profile photo
7. Observe behavior

## Actual Result
The application crashes after uploading a profile photo.

## Expected Result
The application should upload the photo successfully and proceed to the next step without crashing.

## Severity
Critical

## Priority
High

## Frequency
Sometimes

## Impact
Blocks registration for users selecting "Speaker" role.

## Environment:

- Device: Xiaomi Redmi Note 11
- OS: Android 11
- MIUI: 13.0.14
- Build: HeroesSchool-v1.0-debug.apk

## Notes
Possible issue related to role-specific logic or API handling during photo upload.
