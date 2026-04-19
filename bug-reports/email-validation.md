# Bug: API accepts invalid email format and returns success

## Description
-Backend accepts email values with multiple domain levels (e.g., test@1.com.com.com.com.com.com) and processes the request successfully.

-Frontend validation restricts some invalid formats, but backend does not enforce the same rules, leading to inconsistent validation.

## Steps to Reproduce
1. Open Postman
2. Send POST request to /contact
3. Use body:
   {
     "email": "test@1.com.com.com.com.com.com",
     ...
   }
4. Send request
5. Observe response

## Actual Result
API returns success: true and processes request with invalid email.

## Expected Result
System should ensure consistent validation between frontend and backend or apply stricter validation rules if required by product logic.

## Severity
Medium

## Priority
Medium

## Frequency
Always

## Impact
Invalid email data may be stored, reducing data quality and affecting communication with users.

## Attachments:
<img width="693" height="899" alt="image" src="https://github.com/user-attachments/assets/068591f7-522e-42f5-b579-ada6ba694df1" />


## Environment:
- Device: Xiaomi Redmi Note 11
- OS: Android 11
- MIUI: 13.0.14
- Build: HeroesSchool-v1.0-debug.apk

## Notes
According to RFC standards, such email format may be technically valid, but not realistic. Consider stricter validation rules.
