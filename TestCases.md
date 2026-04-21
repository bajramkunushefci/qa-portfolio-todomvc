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