# Test Case ID: RES-0001
## Test Case Name: Book reservation - Submit

**Summary:** Verify that an authenticated user can successfully submit a reservation request for an available library book.

**Preconditions:**
1. The user is logged into their account.
2. The targeted book record is currently set to "available".

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Navigate to the book detail page and click the "Reserve Book" button. | Verify that a reservation form or confirmation modal appears displaying the correct book details. |
| 2 | Select a valid future collection date and click the "Confirm Reservation" button. | Verify that a success notification is displayed and the reservation transaction is logged in the system database. |