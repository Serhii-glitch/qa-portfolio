# Schedule (Events) Checklist

## Scope
Testing events list, event details navigation, UI, and behavior under different conditions.

---

## General

- [ ] Page loads without errors
- [ ] Events are displayed with correct data
- [ ] Event cards display correctly on different screen sizes

---

## Event Information

- [ ] Event title is displayed correctly
- [ ] Event date and time are correct
- [ ] Event location is displayed correctly
- [ ] Event image is displayed
- [ ] Long descriptions are truncated correctly

---

## Event Details (Button "Details")

- [ ] "Details" button is visible on each event card
- [ ] Button is clickable
- [ ] Clicking opens event details page or modal
- [ ] Correct event data is opened
- [ ] URL changes correctly after navigation

---

## UI / UX

- [ ] Buttons have correct hover and active states
- [ ] Text is readable
- [ ] Layout is not broken

---

## Edge Cases

- [ ] Event without image is displayed correctly
- [ ] Event with long title does not break layout
- [ ] Empty state is handled (no events message)

---

## Negative

- [ ] Multiple rapid clicks on "Details" do not break navigation
- [ ] Clicking during loading does not cause errors

---

## Network / Performance

- [ ] Page loads correctly on slow internet
- [ ] Behavior is correct when connection is lost
- [ ] Page refresh during loading does not break functionality
- [ ] Network interruptions are handled gracefully
