# Exploratory Testing

## Overview
This document contains notes from exploratory testing done on the React TodoMVC application. The goal was to freely test the app and observe any unexpected behavior or issues.

## What was tested
- Adding multiple todos quickly
- Editing and deleting todos
- Using long text in todos
- Switching between filters
- Refreshing the page after actions
- General UI behavior and interactions

## Observations

### 1. Long todo text UI issue (UI bug)
When a very long todo is added, the delete ("x") button becomes hard to see and difficult to click. It overlaps the todo text when hovering and makes it harder to find.

This makes it difficult to delete long todos properly.

### 2. General behavior
- Basic todo actions work as expected
- No major crashes or broken screens found during testing
- UI becomes less usable with long input values

## Conclusion
Exploratory testing helped find a UI issue related to long text handling. The application works normally for short and medium inputs, but usability decreases when long todos are used.