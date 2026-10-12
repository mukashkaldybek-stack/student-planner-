# Student Planner — Development Process

## 1. Purpose

This document defines the workflow for developing Student Planner using AI-assisted development.

## 2. Source of Truth

- `_docs/plan.md` defines the project scope and requirements.
- GitHub Issues are the official task backlog.
- `AGENTS.md` defines general AI development rules.

## 3. Team Roles

### Product Manager (PM)

- Reviews and clarifies task requirements.
- Defines a clear goal and testable acceptance criteria.
- Identifies edge cases and out-of-scope work.
- Uses `_docs/task-template.md`.
- Does not write application code.

### Software Engineer

- Implements one approved GitHub Issue at a time.
- Follows acceptance criteria and project constraints.
- Writes tests and runs them.
- Commits changes regularly.
- Reports completed work in the issue.
- Does not close the issue.

### QA Engineer

- Checks every acceptance criterion against the implementation.
- Runs relevant tests.
- Reports PASS or FAIL with evidence.
- Does not fix the implementation.
- Does not close the issue.

## 4. Workflow

For each GitHub Issue:

1. Select the next issue from the backlog.
2. PM reviews and prepares the issue.
3. Engineer implements the task.
4. Engineer runs tests and commits the changes.
5. QA checks the acceptance criteria and test results.
6. If QA reports FAIL, the Engineer fixes the problems and QA checks again.
7. If QA reports PASS, the orchestrator closes the issue.
8. Continue with the next issue until the backlog is complete.

## 5. Completion Rules

An issue can be closed only when:
- All acceptance criteria are satisfied.
- Relevant tests have been run.
- QA reports PASS.
- Evidence is recorded in the issue comments.

## 6. General Principles

- Work on one issue at a time.
- Keep tasks small and understandable.
- Do not skip the PM, Engineer, or QA steps.
- Do not implement unrelated features.
- Keep documentation and code consistent.
