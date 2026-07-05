# Notebook Rules

## Purpose

Keep notebooks understandable, reproducible, and safe for research workflows.

## Rules

- One notebook should have one purpose.
- Do not hide business logic inside notebooks.
- Move reusable code into `src/`.
- Avoid duplicated preprocessing.
- Avoid hidden execution-order dependencies.
- Restart-and-run-all should succeed.
- Record dataset and config used.

## Good Notebook Structure

```text
1. Purpose
2. Imports
3. Configuration
4. Data loading
5. Analysis or experiment
6. Results
7. Conclusion
```

## Bad Behavior

Do not rely on variables created in old cells.

Do not manually patch results in output cells.

Do not leave unclear temporary experiments mixed with final results.

## Checklist

- [ ] Purpose stated
- [ ] Config visible
- [ ] Reusable logic moved to source files
- [ ] Restart-and-run-all works
- [ ] Results are reproducible
