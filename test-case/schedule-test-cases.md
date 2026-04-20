# Schedule (Events) Test Cases

## Scope
Test cases covering events list display, event details navigation, UI behavior, and system behavior under different conditions.

---

### TC-01: Schedule page loads successfully

**Preconditions:**
- User navigates to Schedule page

**Steps:**
1. Open Schedule page

**Expected Result:**
- Page loads without errors
- Events are displayed
- UI is not broken

---

### TC-02: Event data is displayed correctly

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Observe event cards

**Expected Result:**
- Event title is displayed correctly
- Event date and time are correct
- Event location is displayed
- Event image is shown

---

### TC-03: Event card UI responsiveness

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Resize screen or use different devices
2. Observe event cards

**Expected Result:**
- Cards adapt to screen size
- Layout remains consistent
- No overlapping elements

---

### TC-04: Open event details

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Click "Details" button on any event

**Expected Result:**
- Event details page or modal is opened
- Correct event data is displayed
- URL updates correctly (if applicable)

---

### TC-05: "Details" button functionality

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Locate "Details" button on event card
2. Click the button

**Expected Result:**
- Button is clickable
- Navigation works correctly
- No errors occur

---

### TC-06: Event without image

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Find event without image (or simulate)

**Expected Result:**
- Event card is displayed correctly
- Layout is not broken
- Placeholder or empty state is handled properly

---

### TC-07: Long event title handling

**Preconditions:**
- User is on Schedule page

**Test Data:**
Event with very long title

**Steps:**
1. Observe event with long title

**Expected Result:**
- Text is truncated or wrapped correctly
- Layout is not broken

---

### TC-08: Empty events list

**Preconditions:**
- No events available (or simulate empty state)

**Steps:**
1. Open Schedule page

**Expected Result:**
- Appropriate message is displayed (e.g., "No events")
- UI remains consistent

---

### TC-09: Multiple rapid clicks on "Details"

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Click "Details" button multiple times quickly

**Expected Result:**
- Only one navigation action is triggered
- No duplicate pages/modals
- No errors occur

---

### TC-10: Behavior on slow internet connection

**Preconditions:**
- Network throttling enabled (Slow 3G)
- User is on Schedule page

**Steps:**
1. Open Schedule page

**Expected Result:**
- Loading indicator is displayed
- Data loads correctly
- UI does not freeze

---

### TC-11: Behavior with network interruption

**Preconditions:**
- User is on Schedule page

**Steps:**
1. Disable internet connection
2. Refresh page or try to load events

**Expected Result:**
- Error state is handled correctly
- User sees appropriate message
- Application does not crash

---

### TC-12: Page refresh during loading

**Preconditions:**
- User is loading Schedule page

**Steps:**
1. Refresh page while data is loading

**Expected Result:**
- Page reloads correctly
- No duplicated or corrupted data
- Application remains stable
