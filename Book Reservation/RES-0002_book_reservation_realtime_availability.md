# Test Case ID: RES-0002
## Test Case Name: Book reservation - Realtime Availability

**Summary:** Verify that the system dynamically displays the real-time availability status (available, borrowed, or reserved) of books on the catalog interface.

**Preconditions:**
1. The user has navigated to the library book catalog screen.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | View the status indicators on the listed book items in the catalog UI grid. | Verify that each book clearly displays its current real-time status tag ("Available", "Borrowed", or "Reserved"). |
| 2 | Submit a new reservation for a book that was previously marked as "Available". | Verify that the catalog interface updates immediately, changing that specific book's status indicator from "Available" to "Reserved". |