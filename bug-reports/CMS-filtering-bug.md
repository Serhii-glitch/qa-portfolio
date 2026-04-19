# Bug: CMS: Filters do not apply correctly when selecting multiple criteria

## Steps to reproduce:

1) Go to the events page in the CMS.

2) In the “Event type” filter, select “Internship.”

3) Open any event from the filtered list.

4) Return to the events list.

## Actual result:
The “Internship” filter remains applied to the events list, but the filter no longer shows that this option is selected (the checkmark disappears).

## Expected result:

If the filter is applied, it should remain checked in the filter.

## Location
CMS → Events page (filter section)

## Frequency
Always

## Priority:

Medium

## Severity:

Major

## Additional information:
The same behavior is observed with the “Job” filter.

## Environment:
Google Chrome Version 146.0.7680.81 (Official Build) (64-bit)

## Attachments:

https://github.com/user-attachments/assets/a08bd54e-ba30-4a93-bea9-d8751a14b712

## Notes
This issue may indicate incorrect filtering logic on the backend or missing combination handling for multiple filters.

