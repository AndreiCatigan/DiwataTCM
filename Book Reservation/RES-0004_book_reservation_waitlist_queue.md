# Test Case ID: RES-0004
## Test Case Name: Book Reservation - Waitlist Queue Handshake

**Summary:** Verify that attempting to reserve a catalog item during a completely full calendar range securely triggers the waitlist fallback sequence.

**Preconditions:**
1. The student is logged in and viewing a book detail panel whose calendar periods all report "0 open" availability records.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Open the reservation calendar modal and select a date within an entirely unavailable window range. | Verify the modal summary notes: "No stock for the full selected period". |
| 2 | Click the action button, which has dynamically adapted to display the text label "Join waitlist". | Verify the modal drops, the transaction is processed via the database RPC with `join_queue_when_full` set to true, and a success message indicates placement on the waitlist. |