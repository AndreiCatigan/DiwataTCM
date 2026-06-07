# Test Case ID: SRCH-0002
## Test Case Name: Book search - Author

**Summary:** Verify that the system successfully filters and displays all book records written by a specific author string query.

**Preconditions:**
1. The user has navigated to the library book search interface.
2. Book records written by the queried author exist in the library database.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click on the main search input bar field. | Verify that the field is active and ready for text input. |
| 2 | Type a valid author's name (e.g., "Ian Sommerville") into the input field and click the "Search" button. | Verify that the system processes the request and displays all available book records attributed to that specific author. |