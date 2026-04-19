# Bug: Login button is triggered when tapping outside the button area

## Location
Login / Registration screen

## Description
-Tapping on an empty area near the "Login" button triggers the button action.

-There appears to be an invisible clickable zone extending beyond the visible button boundaries.

## Steps to Reproduce
1. Open Login or Registration screen
2. Do not enter any data
3. Tap on an empty area near the "Login" button (outside visible button bounds)
4. Observe behavior

## Actual Result
The "Login" button is triggered even when tapping outside its visible area.

## Expected Result
Button should be triggered only when tapping directly on the visible button area.

## Severity
Major

## Priority
High

## Frequency
Always

## Impact
Users may accidentally trigger actions, leading to unintended behavior and poor user experience.


## Environment:

Device: Xiaomi Redmi Note 11
OS: Android 11
MIUI: 13.0.14
Build: HeroesSchool-v1.0-debug.apk

## Attachments:

https://github.com/user-attachments/assets/6ac09441-0f3a-47fd-a8b8-24255d9b3b20

## Notes
Possible issue with incorrect layout bounds or overlapping clickable elements.
