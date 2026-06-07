# Test Case ID: RES-0001
## Test Case Name: Book reservation - Submit

**Summary:** Verify that an authenticated student can successfully schedule a book pickup using the reservation calendar modal.

**Preconditions:**
1. The user is logged in and viewing a valid book details page.
2. The book has `available_copies > 0`[cite: 1].

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click the primary "Reserve this book" action button[cite: 1]. | Verify that a reservation calendar modal opens, displaying the book title and a 7-day pickup selection grid[cite: 1]. |
| 2 | Click on a calendar day marked as "available" (e.g., "1 open")[cite: 1]. | Verify the selected date gets a green focus ring and the summary updates to show the 7-day reservation period[cite: 1]. |
| 3 | Click the "Confirm reservation" button[cite: 1]. | Verify the modal closes, a success toast displays "Reservation confirmed. You may pick it up starting on your selected date.", and the main button updates to "Reserved"[cite: 1]. |