# Test Case ID: ADMIN-0002
## Test Case Name: Admin - Add New Book Inventory

**Summary:** Verify that a librarian can successfully add a new physical book record to the system's catalog.

**Preconditions:**
1. The administrator is logged in and viewing the "Inventory / Catalog Manager" page (`/admin-inventory`)[cite: 1].

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Click the "Add Book" button located in the top toolbar[cite: 1]. | Verify that the `BookForm` modal opens overlaying the screen[cite: 1]. |
| 2 | Fill out the required text fields (Title, Author, ISBN), select a Category and Status, specify the total copies, and optionally upload a cover photo[cite: 1]. | Verify the form inputs accept the data and the cover photo generates a local preview[cite: 1]. |
| 3 | Click the "Save Book" button[cite: 1]. | Verify the modal closes, the database inserts the new book record, and the catalog table refreshes to display the newly added item[cite: 1]. |