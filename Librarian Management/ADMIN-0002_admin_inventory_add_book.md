# Test Case ID: ADMIN-0002
## Test Case Name: Admin - Add New Book Inventory

**Summary:** Verify that a librarian can successfully add a new physical book record to the system's catalog.

**Preconditions:**
1. The administrator is logged in and viewing the "Inventory / Catalog Manager" page (`/admin-inventory`).

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click the "Add Book" button located in the top toolbar. | Verify that the `BookForm` modal opens overlaying the screen. |
| 2 | Fill out the required text fields (Title, Author, ISBN), select a Category and Status, specify the total copies, and optionally upload a cover photo. | Verify the form inputs accept the data and the cover photo generates a local preview. |
| 3 | Click the "Save Book" button. | Verify the modal closes, the database inserts the new book record, and the catalog table refreshes to display the newly added item. |