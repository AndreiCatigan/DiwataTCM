# Test Case ID: ADMIN-0001
## Test Case Name: Admin - Process Checkout (Picked Up)

**Summary:** Verify that an administrator can successfully process a student's book pickup from the Circulation queue.

**Preconditions:**
1. The administrator is logged into the `/admin` portal.
2. The administrator has navigated to the "Circulation / Load" page (`/admin-circulation`)[cite: 1].
3. A reservation exists in the queue with a status of "reserved", "approved", or "ready_for_pickup"[cite: 1].

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Locate the target reservation in the "Pickup queue" list and verify the student's ID and email[cite: 1]. | Verify the record displays the correct book, student details, and reservation timeline[cite: 1]. |
| 2 | Click the primary "Picked Up" action button on the reservation card[cite: 1]. | Verify that the system executes the `admin_mark_reservation_picked_up` procedure, converts the reservation into an active loan, and removes it from the pickup queue[cite: 1]. |