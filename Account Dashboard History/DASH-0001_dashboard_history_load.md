# Test Case ID: DASH-0001
## Test Case Name: Dashboard - History Load

**Summary:** Verify that the dashboard successfully fetches and displays the authenticated student's historical library records upon loading.

**Preconditions:**
1. The user is logged in and possesses existing borrowing/reservation records in the database.
2. The user navigates to the `/dashboard` route[cite: 1].

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Observe the initial page load state. | Verify the `PortalLiveIndicator` displays "Syncing library history..." while fetching data[cite: 1]. |
| 2 | Review the "Status Shelf" section once loading completes[cite: 1]. | Verify that up to 5 compact transaction cards are rendered, displaying the book cover, title, borrow date, and return date[cite: 1]. |