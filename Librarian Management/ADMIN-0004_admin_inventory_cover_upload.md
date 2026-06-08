# Test Case ID: ADMIN-0004
## Test Case Name: Admin - Drag and Drop Cover Photo Storage

**Summary:** Verify that administrators can bind visual cover files to catalog books using interactive drag-and-drop input listeners.

**Preconditions:**
1. The librarian is logged in and has initialized the `BookForm` rendering workspace.

| # | Step Actions | Expected Results |
|---|---|---|
| 1 | Drag an image asset from a local file directory and drop it directly onto the dashed boundary target area of the form. | Verify the workspace intercepts the drop event, maps the object to an active layout preview, and uploads the file to the Supabase storage bucket. |
| 2 | Observe the upload statement and check row tracking links. | Verify the feedback row prints "Cover uploaded." and updates the asset text field with the verified live public storage URL. |