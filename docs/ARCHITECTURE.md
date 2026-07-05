# Architecture

## Purpose

Guide AI coding agents to understand the project structure before making design or implementation changes.

## Rules

- Understand existing layers before adding new code.
- Reuse existing abstractions.
- Avoid parallel implementations.
- Keep business logic out of notebooks.
- Keep reusable code inside source modules.
- Keep configuration outside hardcoded logic.
- Avoid hidden global state.

## Preferred AI/ML Flow

```text
Dataset
→ DataLoader
→ Model
→ Loss
→ Trainer
→ Evaluation
```

## Good Behavior

Before adding a new class or module, search for:

- existing classes with similar responsibility
- existing factories
- existing config objects
- existing tests

## Bad Behavior

Do not create a new abstraction just because the current task is slightly different.

Do not rewrite architecture unless the user explicitly asks.

## Checklist

- [ ] Existing structure inspected
- [ ] Similar modules searched
- [ ] Public interfaces preserved
- [ ] New code placed in correct layer
- [ ] No duplicated architecture introduced
