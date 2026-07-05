# Testing

## Purpose

Ensure AI-generated changes are verified before they are treated as complete.

## Rule

Never claim success without verification.

## Preferred Commands

Use the commands defined by the project.

Common examples:

```bash
pytest
ruff check .
mypy .
```

Do not invent commands. Inspect the repository first.

## If Tests Fail

Report:

- command run
- failure summary
- likely cause
- whether the failure is related to the change
- next suggested fix

## If Tests Cannot Run

State why:

- missing dependency
- missing dataset
- missing environment variable
- unavailable service
- command not defined

## Completion Checklist

- [ ] Relevant tests run
- [ ] Lint run if available
- [ ] Type check run if available
- [ ] Failures reported honestly
- [ ] No unverified success claim
