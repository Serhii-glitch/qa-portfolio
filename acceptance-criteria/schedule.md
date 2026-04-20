# Schedule – Acceptance Criteria

## Scope
Acceptance criteria for Events (Schedule) functionality including filtering, search, sorting, and pagination.

---

## General

- User can view list of all events
- User can search events
- User can filter events by:
  - City
  - Date
  - Event format
  - Manager
  - Time

---

## City Filter

- Default value is "All cities"
- Dropdown contains trending cities (Kyiv, Lviv, etc.)
- User can:
  - Select city from dropdown
  - Type city manually
- Filtering works with:
  - Exact match
  - Partial match
  - Case-insensitive input
- Invalid input returns empty result
- If no events → "No events" message is displayed
- Selected city replaces default value
- Filter works together with other filters

---

## Event Format Filter

- Dropdown contains available formats
- User can:
  - Select one format
  - Select multiple formats
- Results update accordingly
- "Any format" resets filtering
- No results → appropriate message
- Selection persists after page reload (if required)

---

## Date Filter

- User can filter by specific date
- User can filter:
  - Past events
  - Future events
  - Today
- Results update based on selected date
- No results → appropriate message

---

## Manager Filter

- Dropdown contains list of managers
- User can:
  - Select one or multiple managers
- Search works by partial match
- Results update accordingly

---

## Sorting

- Default: Newest first
- User can change sorting order:
  - New → Old
  - Old → New
- Events reorder accordingly

---

## Pagination

- User can select number of items per page:
  - 10, 15, 20, 25, 50, 100
- Pagination appears when needed
- Pagination disappears if all items fit on one page
- Filters persist after changing page size

---

## Bulk Actions

- Each event has checkbox
- "Select all" checkbox is available
- User can perform actions:
  - Edit
  - Delete
  - Copy
  - Hide

---

## Additional

- User can open side panel with icons
- "Clear filters" resets all filters to default
- User can create a new event
