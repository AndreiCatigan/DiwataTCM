# Test Case ID: AUTH-0004
## Test Case Name: Authentication - Password Strength Meter

**Summary:** Verify that the real-time password strength tracker dynamically adjusts meter-track fill percentages and styling classes based on string complexity.

**Preconditions:**
1. The user has navigated to the `/` auth route and toggled the active mode to "Sign Up".

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Focus the Password input field and type a simple string (e.g., "123"). | Verify the strength track displays a weak indicator mapping to the `.meter-fill.score-0` or `.meter-fill.score-1` configuration. |
| 2 | Append uppercase letters, numbers, and non-alphanumeric symbols to the password field (e.g., "P@ssword2026"). | Verify the track transitions fluidly through score thresholds, hitting 100% width and rendering the vibrant emerald style on the `.meter-fill.score-4` element. |