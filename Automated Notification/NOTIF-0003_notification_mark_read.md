# Test Case ID: NOTIF-0003
## Test Case Name: Notification - Mark as Read

**Summary:** Verify that interacting with notifications correctly updates their read status and clears the unread badge count.

**Preconditions:**
1. The user is logged in and has the notification panel open.
2. The user has multiple unread notifications.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click directly on a single unread notification item within the list. | Verify that the specific item loses its unread styling, and the main notification badge count decreases by exactly 1[cite: 1]. |
| 2 | Click the "Mark all as read" link (`.notifier-link`) inside the notification panel header[cite: 1]. | Verify that all remaining unread items instantly switch to the read state, and the red notification badge disappears completely from the bell icon[cite: 1]. |