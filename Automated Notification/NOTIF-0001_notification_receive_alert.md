# Test Case ID: NOTIF-0001
## Test Case Name: Notification - Receive Alert

**Summary:** Verify that the system successfully delivers a real-time notification to the user when a reservation status changes.

**Preconditions:**
1. The student is logged into the application and viewing any main portal page (e.g., Dashboard or Search).
2. The user has an active reservation pending approval.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Have a librarian/admin account approve the user's pending reservation from the admin circulation panel. | Verify that a real-time toast popup (`.notifier-toast`) animates onto the screen displaying the approval message. |
| 2 | Observe the notification bell icon in the top navigation bar. | Verify that the red unread badge (`.notifier-badge`) increments its count to reflect the new alert. |