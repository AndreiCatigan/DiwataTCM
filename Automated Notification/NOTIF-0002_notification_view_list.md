# Test Case ID: NOTIF-0002
## Test Case Name: Notification - View List

**Summary:** Verify that a user can open the notification panel to view their historical and unread alerts.

**Preconditions:**
1. The user is logged in.
2. The user has at least one unread notification and several historical notifications.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click the notification bell toggle (`.notifier-toggle`) in the top navigation bar[cite: 1]. | Verify that the notification panel drops down, displaying a scrollable list of recent alerts[cite: 1]. |
| 2 | Inspect the visual styling of the listed items. | Verify that unread items are distinctly highlighted (e.g., green tint/border via `.notifier-item.unread`), while read items have a standard white background[cite: 1]. |