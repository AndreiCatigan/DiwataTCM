# Test Case ID: AUTH-0001
## Test Case Name: User authentication - Gmail Signup

**Summary:** Verify that a user can successfully create an account when submitting a registration form with a valid Gmail address.

**Preconditions:**
1. The user has opened the registration view on a supported web browser.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Fill out the name, a valid Gmail address, and a secure password in the registration fields. | Verify that the input values are accepted and characters in the password field are masked. |
| 2 | Click the "Create Account" button. | Verify that the system communicates with the Authentication API and displays a prompt to check the user's email inbox. |