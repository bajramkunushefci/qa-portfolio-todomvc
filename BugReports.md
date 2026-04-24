# Bug Reports

---

## BUG-001 — Single-character todo input not accepted without feedback

Title: Single-character todo input is ignored without user feedback

Severity: Low / Medium (UX issue)

Priority: Medium

Steps to reproduce:
Enter “A”
Press Enter

Actual Result:
No todo is created and no message is shown

Expected Result:
Either:
Todo should be created, OR
User should receive validation feedback explaining requirement


Notes:
Multi-character inputs work as expected
Suggests implicit validation rule exists but is not communicated



## BUG-02 — Escape key does not cancel edit mode

Title: Escape key does not exit edit mode or revert changes

Severity: Medium (Functional defect)

Priority: High (core interaction broken)

Steps to reproduce:
Add a todo
Double-click to edit
Modify text
Press Escape

Actual result:
No response to Escape key
Edit mode remains active
Modified text stays visible

Expected result:
Edit mode should close
Original text should be restored
No changes should be saved

## BUG-03 — Todos are not persisted after page reload

Title: Todo items are lost after browser refresh (no persistence)

Severity: High

Priority: High

Steps to reproduce:
Open TodoMVC app
Add multiple todos
Confirm todos appear in UI
Refresh browser page

Actual result:
All todos are removed after refresh
Application resets to initial empty state

Expected result:
Todos should persist across page reloads
Previously entered data should be restored from storage

Additional reproduction paths:
Create todos → refresh → data lost
Edit todo → refresh → data lost