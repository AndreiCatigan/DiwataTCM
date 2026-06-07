# Test Case ID: AUTH-0002
## Test Case Name: User authentication - Invalid Email

**Summary:** Verify that the system rejects the registration request if the format of the email address is invalid.

**Preconditions:**
1. The user has opened the registration view on a supported web browser.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Enter a syntactically invalid email string (e.g., "andreigmail.com" missing the @ symbol) into the email field. | Verify that the field accepts the text characters. |
| 2 | Click the "Create Account" button. | Verify that the application blocks transmission to the Authentication API and displays an inline red validation error below the input field. |