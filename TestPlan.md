# Test Plan — React TodoMVC

## 1. Overview

This document describes how I tested the React TodoMVC application. The goal was to check if the main features work correctly and to find any bugs or issues in normal and edge use.

## 2. Objectives

* Verify create, edit, delete, and complete todo actions
* Check filters (All, Active, Completed)
* Check behavior with invalid inputs
* Verify data persistence after page reload
* Record results and report bugs

## 3. Scope

**In Scope:**

* Add, edit, delete todos
* Mark complete/incomplete
* Filters (All/Active/Completed)
* LocalStorage persistence
* Basic UI behavior and keyboard actions (Enter, Escape, Tab)

**Out of Scope:**

* Performance testing
* Security testing
* Backend/API (not applicable)

## 4. Test Approach

Manual testing was performed using:

* Functional testing (main features)
* Negative testing (empty/invalid input)
* Boundary testing (short and long text)
* State testing (active/completed/delete flows)
* Basic exploratory testing
* Persistence testing using localStorage

## 5. Test Environment

* Browser: Google Chrome (v122)
* OS: Windows 11
* App: React TodoMVC (run locally)

## 6. Test Data

* Normal text (e.g., "Buy milk")
* Single character (e.g., "A")
* Long text (500+ chars)
* Special characters and emojis
* Empty and whitespace input

## 7. Entry Criteria

* App is running locally
* Test cases are ready

## 8. Exit Criteria

* All test cases executed
* Results saved in testexecution.md
* Bugs logged in bugreports.md

## 9. Deliverables

* testplan.md
* testcases.md
* testexecution.md
* bugreports.md

## 10. Risks

* Data may not persist after reload
* Some behaviors may be unclear without requirements
* UI may behave inconsistently in edge cases

## 11. Summary

Testing was done to check real user behavior and find issues. Results and bugs are documented in the repository.
