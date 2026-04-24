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

Actual Result:
The completed todo item is removed from the list

## TC-04: Delete a todo using delete button

Status: Pass

Actual Result:
The todo item is removed from the list and is no longer visible.

## Tc-05: Mark a todo as Completed

Status: Pass

Actual Result:
The todo item is marked as completed, and its text is displayed with a strikethrough style

## TC-06: Verify "Active" filter shows only incomplete todos

Status: Pass

Actual Result:
The "example" todo is no longer visible, now we can only see the "another example" todo.

## TC-07: Verify "Completed" filter shows only completed todos

Status: Pass

Actual Result:
Only the completed todo is displayed

## TC-08: Verify "All" filter shows all todos

Status: Pass

Actual Result:
All todos are displayed regardless of status

## TC-09: Add whitespace-only todo

Status: Pass

Actual Result: Ignored therefore todo not added

## TC-10: Add single-character todo

Status: Pass with observation

Expected Result:
Todo item with text "A" should be created and displayed in the list.

Actual Result:
No todo is created. Pressing Enter has no visible effect.

Notes:
- Input with a single character is ignored.
- No validation message or feedback is shown.
- Behavior differs from multi-character input, where todos are created normally.

## TC-11: Add very long todo (500+ chars)

Status: Pass

Actual Result: Todo is created successfully
No UI break

## TC-12: Add special characters

Status: Pass

Actual Result: Rendered correctly

## TC-13: Add emoji/unicode todo

Status: Pass

Actual Result: Stored and rendered correctly

## TC-14: Edit existing todo

Status: Pass

Actual Result: Updated text saved

## TC-15: Cancel edit using Escape

Status: Fail

Expected Result:
Edit mode should close, and original todo text should be restored without saving changes.

Actual Result:
Pressing Escape has no effect. The todo remains in edit mode and the modified text remains unchanged.

## TC-16: Click outside during edit (blur save/cancel)

Status: Pass

Actual Result: Edit is canceled (Behaviour is consistent)

## TC-17: Reload page after adding todos

Status: Fail

Expected Result:
Previously created todos should persist after page reload via localStorage or equivalent storage mechanism.

Actual Result:
All todos are lost after refresh. The application loads in an empty initial state as if it is being accessed for the first time.

## TC-18: Edit then reload

Status: Fail

Expected Result:
Edited todo should persist after reload with updated text preserved.

Actual Result:
All todos are lost after refresh. Application resets to empty state.