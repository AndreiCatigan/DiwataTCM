# Test Case ID: ADMIN-0003
## Test Case Name: Admin - Apply User Restriction

**Summary:** Verify that an administrator can suspend a student's library privileges due to policy violations or excessive fines.

**Preconditions:**
1. The administrator is logged in and viewing the "Users & Penalties" page (`/admin-users`)[cite: 1].
2. The targeted user currently has an "Active" or "Restricted" account status[cite: 1].

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Locate the target student in the User Records table and click the "Restrict" button[cite: 1]. | Verify the `RestrictModal` opens, displaying the student's name, a text area for the reason, and a duration dropdown[cite: 1]. |
| 2 | Input a custom restriction reason, select a duration (e.g., "7 Days"), and click "Apply Restriction"[cite: 1]. | Verify the system updates the user's `account_status` to "suspended", logs the `restricted_until` date in their metadata, sends them a restriction notification, and updates the UI table[cite: 1]. |