## Description:

The contact form allows submission with an invalid email format such as "gmail.com.com.com".

Frontend validation prevents clearly invalid emails, but still allows structurally incorrect email formats.

## Steps:

1) Enter email: test@1.com.com.com.com.com.com
2) Fill other required fields
3) Submit form
4) Actual result:
5) Form is submitted successfully.

## Expected Result:
Email validation should reject invalid formats.

## Severity:

Major

## Attachments:
<img width="693" height="899" alt="image" src="https://github.com/user-attachments/assets/068591f7-522e-42f5-b579-ada6ba694df1" />


## Environment:
- Device: Xiaomi Redmi Note 11
- OS: Android 11
- MIUI: 13.0.14
- Build: HeroesSchool-v1.0-debug.apk
