# Test Case ID: RES-0003
## Test Case Name: Book reservation - Rejection Borrowed

**Summary:** Verify that the system blocks reservation requests and handles errors gracefully when a user attempts to reserve a book currently marked as borrowed.

**Preconditions:**
1. The user is logged into their account.
2. The target book is currently checked out by another student and marked as "borrowed".

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Navigate to a book detail page where the status indicator is explicitly set to "Borrowed". | Verify that the primary "Reserve Book" action button is visually grayed out or disabled. |
| 2 | Attempt to bypass the UI constraint to force a reservation request submission on the borrowed item. | Verify that the system firmly rejects the request, prevents a transaction entry from being made, and displays an error message stating the item is currently unavailable. |