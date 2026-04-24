# Test Cases

---

## TC-01: Add a valid todo

Steps:
1. Type "Buy groceries" in the input field
2. Press Enter key

Expected Result:
A new todo item with the text "Buy groceries" is added to the list

---

## TC-02: Add an empty todo

Steps:
1. Click on the input field
2. Press Enter key without typing anything

Expected Result:
No todo item should be added to the list

---

## TC-03: Remove a completed todo using "Clear completed"

Steps:
1. Add a new todo
2. Mark the todo as complete by clicking the checkbox
3. Click on "Clear completed"

Expected Result:
The completed todo item is removed from the list

---

## TC-04: Delete a todo using delete button

Steps:
1. Add a new todo with text "Test item"
2. Hover over the todo item
3. Click the delete button (X icon)

Expected Result:
The todo item is removed from the list and is no longer visible.

---

## Tc-05: Mark a todo as Completed

Steps: 
1. Add a new todo with text "example"
2. Click the checkbox on todo we just added

Expected Result:
The todo item is marked as completed, and its text is displayed with a strikethrough style

---

## TC-06: Verify "Active" filter shows only incomplete todos

Steps:
1. Add two new todos with text "example" and "another example"
2. Mark the "example" todo as completed
3. Click on the "Active" filter

Expected Result:
The "example" todo is no longer visible, now we can only see the "another example" todo.

--

## TC-07: Verify "Completed" filter shows only completed todos

Steps:
1. Add two todos
2. Mark one as completed
3. Click "Completed" filter

Expected Result:
Only the completed todo is displayed

---

## TC-08: Verify "All" filter shows all todos

Steps:
1. Add multiple todos
2. Mark some as completed
3. Click "All" filter

Expected Result:
All todos are displayed regardless of status

## TC-09: Add whitespace-only todo

Steps:
1. Enter " "
2. Press Enter

Expected: Ignored OR trimmed and not added

## TC-10: Add single-character todo

Steps:
1. Enter “A”
2. Press Enter

Expected: Todo created

## TC-11: Add very long todo (500+ chars)

Steps:
1. Type a long string (500–1000 chars)
2. Press Enter

Expected:
Todo is created successfully
No UI break

## TC-12: Add special characters

Steps:
1. Enter "@#$%^&*()_+{}|"
2. Press Enter

Expected: Rendered correctly

## TC-13: Add emoji/unicode todo

Steps:
1. Enter “🔥 Test 测试 مرحبا”
2. Press Enter

Expected: Stored and rendered correctly

## TC-14: Edit existing todo

Steps:
1. Double-click an existing todo
2. Modify text
3. Press Enter

Expected: Updated text saved

## TC-15: Cancel edit using Escape

Steps:
1. Double-click todo
2. Modify text
3. Press Escape

Expected: Original text restored

## TC-16: Click outside during edit (blur save/cancel)

Steps:
1. Edit todo
2. Click outside input

Expected: Behavior consistent (save or cancel, defined by app)

## TC-17: Reload page after adding todos

Expected: Todos persist

## TC-18: Edit then reload

Expected: Edited data persists