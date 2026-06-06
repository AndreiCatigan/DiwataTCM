# Test Case ID: DW_AUTH_02
## Test Case Name: Account Creation Rejection via Invalid Email Format

**Summary:** Verify that the system rejects account creation requests and displays a clear validation error when the input email string format is syntactically invalid.

**Preconditions:**
1. The user must navigate to the registration portal on a supported browser.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Locate the registration form and input a valid name, an invalid email string (e.g., "andreicatigangmail.com" missing the @ symbol), and a secure password. | Verify that the text fields accept the raw keystroke strings. |
| 2 | Click the "Create Account" button. | Verify that the system blocks the request from firing to the external Authentication API, prevents form disabling, and does not show a loading spinner. |
| 3 | Observe the client-side user interface state. | Verify that a red inline validation error message appears immediately below the email field stating "Please enter a valid email address". |