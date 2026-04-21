# Test Execution

---

## TC-01: Add a valid todo

Status: Pass

Actual Result:
Todo was successfully added to the list

## TC-02: Add an empty todo

Status: Pass

Actual Result:
No todo item is added to the list

## TC-03: Remove a completed todo using "Clear completed"

Status: Pass

Expected Result:
The completed todo item is removed from the list

## TC-04: Delete a todo using delete button

Status: Pass

Actual Result:
The todo item is removed from the list and is no longer visible.

## Tc-05: Mark a todo as Completed

Status: Pass

Expected Result:
The todo item is marked as completed, and its text is displayed with a strikethrough style

## TC-06: Verify "Active" filter shows only incomplete todos

Status: Pass

Expected Result:
The "example" todo is no longer visible, now we can only see the "another example" todo.

## TC-07: Verify "Completed" filter shows only completed todos

Status: Pass

Expected Result:
Only the completed todo is displayed

## TC-08: Verify "All" filter shows all todos

Status: Pass

Expected Result:
All todos are displayed regardless of status.