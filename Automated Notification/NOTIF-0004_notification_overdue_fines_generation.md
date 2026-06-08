# Test Case ID: NOTIF-0004
## Test Case Name: Notification - Automated Overdue Trigger

**Summary:** Verify that the system automatically shifts active loan tags to overdue and triggers appropriate alerting payloads when a due date threshold passes.

**Preconditions:**
1. An active loan transaction row exists in the database where `due_at` is older than the current date timestamp.
2. The assigned student logs into the portal workspace.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Log in as the student holding the expired item and monitor the notification feed bell icon. | Verify that two notification entities are created: an in-app `loan_overdue` item and an email-queued alerting artifact. |
| 2 | Expand the notification text detail pane and review the auto-generated currency values. | Verify the message body details the accrued penalties calculated strictly against the admin configuration formula (Days Overdue × Fine Rate). |