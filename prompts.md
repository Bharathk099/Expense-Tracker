# Expense Tracker — Prompt Library

## 1. New Feature Prompt
**Context:** This project uses React and Vite. Follow the instructions in AGENTS.md.

**Goal:** Implement the requested feature: [describe feature].

**Constraints:** Keep the change scoped, use existing conventions, avoid unnecessary dependencies, and work on a feature branch.

**Acceptance Criteria:**
- The feature behaves as specified.
- Invalid inputs and edge cases are handled.
- Relevant automated tests pass.
- Existing functionality continues to work.

**Examples:** Describe expected input, action, and output.

First propose a plan and wait for approval.

## 2. Bug Fix Prompt
**Context:** Describe the affected component and observed behavior.

**Goal:** Identify and fix the underlying cause.

**Constraints:** Do not hide the error, weaken tests, or modify unrelated files.

**Acceptance Criteria:** Reproduce the bug, add or update a regression test, fix it, and run relevant tests.

**Examples:** Include the steps to reproduce and the expected versus actual behavior.

Inspect first and propose a plan before editing.

## 3. Refactoring Prompt
**Context:** Identify the code to refactor.

**Goal:** Improve readability and maintainability without changing behavior.

**Constraints:** Preserve public interfaces and existing requirements. Do not add dependencies without approval.

**Acceptance Criteria:** Existing tests pass, behavior remains unchanged, and the diff stays focused.

**Examples:** Show the current problem and the desired improvement.

Propose the refactoring plan before making changes.

## 4. Generate Tests Prompt
**Context:** Identify the component or utility and its expected behavior.

**Goal:** Create meaningful unit, component, or end-to-end tests.

**Constraints:** Do not change production code or weaken assertions just to make tests pass.

**Acceptance Criteria:** Cover normal cases, invalid input, boundary values, and relevant edge cases. Confirm that tests fail for the intended reason when the behavior is broken.

**Examples:** Include representative inputs and expected outputs.

List the proposed test cases before implementation.

## 5. Review Diff Prompt
**Context:** Review the current branch against its base branch.

**Goal:** Identify bugs, requirement mismatches, security concerns, missing tests, and unnecessary changes.

**Constraints:** Do not modify files during the review.

**Acceptance Criteria:** Report findings by severity, reference affected files or lines, and state which tests were actually run.

**Examples:** Explain the problematic behavior and a suggested correction.

Return the review findings before proposing fixes.

## 6. Commit Message Prompt
**Context:** Summarize the changes in the reviewed Git diff.

**Goal:** Suggest a concise conventional commit message.

**Constraints:** Do not stage, commit, or push anything.

**Acceptance Criteria:** The message accurately describes the changes and uses an appropriate prefix such as feat, fix, test, docs, or chore.

**Examples:** `docs: add coding agent instructions`

Return the proposed message and a brief explanation.