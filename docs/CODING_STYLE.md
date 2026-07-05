# Coding Style

## Purpose

Keep generated code readable, maintainable, and consistent with the existing repository.

## Rules

Prefer:

- clear names
- small functions
- type hints
- pathlib
- dataclasses where appropriate
- logging instead of print for application code
- explicit error handling

Avoid:

- wildcard imports
- duplicated logic
- magic numbers
- hidden side effects
- unnecessary inheritance
- broad `Any` usage
- premature abstraction

## Function Design

A function should usually do one thing.

If a function needs many flags, consider whether the design is becoming unclear.

## Class Design

A class should have one main responsibility.

Prefer composition over inheritance unless the codebase already uses inheritance for that pattern.

## Dependency Rules

Do not add new dependencies unless explicitly requested or clearly justified.

Before importing a dependency, inspect:

- `pyproject.toml`
- `requirements.txt`
- `environment.yml`
- existing imports

## Checklist

- [ ] Names are clear
- [ ] Types are explicit where useful
- [ ] No unnecessary dependency added
- [ ] No duplicate helper created
- [ ] Code follows nearby style
