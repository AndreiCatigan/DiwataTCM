# Test Case ID: DW_AUTH_01
## Test Case Name: Account Creation with Valid Gmail Address

**Summary:** 
Verify that a user can successfully create an account when using a valid, standard Gmail address.

**Preconditions:**
1. The user must navigate to the registration portal on a supported browser.
2. The user must possess an active, accessible Gmail account (e.g., @gmail.com).

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Locate the registration form and input a valid name, a standard Gmail address, and a secure password. | Verify that the text fields accept the input data and characters in the password field are securely masked. |
| 2 | Click the "Create Account" button. | Verify that the system disables the form, displays a loading spinner, and fires a request to the external Authentication API. |
| 3 | Check the user interface state after the API response returns. | Verify that a success alert box is displayed instructing the user to check their email, and the system sets the account status to "Pending Verification". |