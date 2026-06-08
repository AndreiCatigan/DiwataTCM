# Test Case ID: RES-0003
## Test Case Name: Book reservation - Rejection Borrowed & Duplicates

**Summary:** Verify that the UI safely disables reservation actions for out-of-stock items and the backend explicitly rejects duplicate active reservation attempts.

**Preconditions:**
1. The user is logged into their account.
2. The user already holds an active reservation for the target book, or the book has 0 available copies.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Navigate to the book details page of the targeted unavailable item. | Verify that the primary reserve button is disabled (unclickable) and explicitly labeled as "Reserved" or "Unavailable". |
| 2 | Force a backend submission attempt (e.g., simulating the `create_student_reservation` RPC call) for a book the user already holds. | Verify the database rejects the transaction and the UI safely catches the error, displaying: "You already have an active reservation for this book.". |