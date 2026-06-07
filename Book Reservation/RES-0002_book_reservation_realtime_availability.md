# Test Case ID: RES-0002
## Test Case Name: Book reservation - Realtime Availability

**Summary:** Verify that the system dynamically syncs and displays exact real-time availability states across the application without requiring a manual page refresh.

**Preconditions:**
1. The user has navigated to the main library catalog or a specific book details page.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | View the availability pill and copy count metadata on a target book card[cite: 1]. | Verify that the UI clearly displays the current tag ("Available", "Borrowed", or "Reserved") alongside the exact `available/total copies` fraction[cite: 1]. |
| 2 | Have a secondary system/user reserve the final available copy of that target book. | Verify that the `PortalLiveIndicator` briefly shows "Syncing live updates...", and the book's availability pill instantly updates to "Reserved" or "Borrowed" without the user refreshing the browser tab[cite: 1]. |