# Test Case ID: AUTH-0003
## Test Case Name: User authentication - API Verification

**Summary:** Verify that clicking the confirmation link sent to the user's email address successfully activates the account status via the Authentication API.

**Preconditions:**
1. A registration request has been submitted and the account is marked as pending verification.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Open the confirmation message inside the registered Gmail inbox and click the verification link. | Verify that a new tab loads showing a successful token activation message from the Authentication API. |
| 2 | Return to the login interface and input the verified account credentials. | Verify that the system updates the account database state to active and redirects the user to the landing dashboard page. |