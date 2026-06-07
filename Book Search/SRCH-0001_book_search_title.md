# Test Case ID: SRCH-0001
## Test Case Name: Book search - Title

**Summary:** Verify that the system successfully returns accurate book records when a user searches using a valid, specific book title.

**Preconditions:**
1. The user has navigated to the library book search interface.
2. The target book title exists within the school library database.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click on the main search input bar field. | Verify that the focus indicator is active and the field is ready for text input. |
| 2 | Input a valid book title (e.g., "Software Engineering Principles") into the field and click the "Search" button. | Verify that the search grid filters accurately and displays the book record matching the queried title. |