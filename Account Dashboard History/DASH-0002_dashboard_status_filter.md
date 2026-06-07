# Test Case ID: DASH-0002
## Test Case Name: Dashboard - Status Filter

**Summary:** Verify that the user can filter their borrowing history by toggling the distinct status bucket buttons.

**Preconditions:**
1. The user is logged in and viewing the dashboard.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Locate the status filter button row containing: Approved, Picked up, Cancelled, Returned, and Overdue[cite: 1]. | Verify the buttons display the correct count of records for each status bucket[cite: 1]. |
| 2 | Click on the "Returned" status button[cite: 1]. | Verify the button receives an active green styling state, and the grid below instantly filters to only show books mapped to the `returned` status[cite: 1]. |
| 3 | Click on the "Overdue" status button[cite: 1]. | Verify the grid updates to show overdue items, or displays the empty state message: "No records are available in this status right now." if none exist[cite: 1]. |