# Test Case ID: DASH-0003
## Test Case Name: Dashboard - Expand Records View

**Summary:** Verify that the "View More" button correctly expands the transaction grid when a status bucket contains more than 5 historical items.

**Preconditions:**
1. The user is logged in and viewing the dashboard.
2. The user has selected a status bucket containing more than 5 records.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Scroll to the bottom of the transaction grid for the active status. | Verify that only 5 items are visible, followed by a final card acting as a "View More (X)" button. |
| 2 | Click the "View More" button. | Verify the grid fully expands to display the remaining items in that status category, and the button text changes to "Show Less". |