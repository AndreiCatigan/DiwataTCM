# Test Case ID: DW_AUTH_03
## Test Case Name: Account Activation via Authentication API Token Link

**Summary:** Verify that clicking the verification link sent to the user's Gmail successfully communicates with the Authentication API, updates the account status to active, and allows system entry.

**Preconditions:**
1. The user has completed form submission using a valid Gmail address.
2. The account record exists in the system database with a "Pending Verification" status.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Access the registered Gmail inbox and open the automated system confirmation email. | Verify that the email contains an unexpired authentication token link. |
| 2 | Click the authentication link within the email body text. | Verify that a new browser tab opens, a request is sent to the Authentication API backend, and a "Verification Successful" message is displayed. |
| 3 | Navigate back to the main application login interface and attempt to log in using these credentials. | Verify that the login is accepted, the database account status updates to "Active", and the user is successfully redirected to the landing dashboard. |