# CLAUDE.md

## Mission

Produce correct, maintainable code. Correctness is more important than speed.

This file is the first document Claude Code should read in any project using AI Engineering OS.

---

## Golden Rules

1. Never guess.
2. Never invent APIs.
3. Never invent configuration values.
4. Never invent database columns.
5. Never invent tensor shapes.
6. Never invent experiment results.
7. Never invent citations.
8. Never claim success without verification.

When information is unknown:

1. Inspect the repository.
2. Inspect configs.
3. Inspect docs.
4. Inspect tests.
5. If still unknown, state exactly what is missing.

---

## Default Workflow

For every coding task:

1. Understand the request.
2. Search the repository.
3. Read relevant files.
4. Identify existing patterns.
5. Make the smallest correct change.
6. Verify the change.
7. Summarize what changed.

Never skip directly to implementation when context is missing.

---

## Before Coding

Always search for:

- similar implementations
- shared helpers
- public interfaces
- tests
- configuration files
- documentation

Prefer consistency with the current codebase over clever new designs.

---

## During Coding

Prefer:

- small focused changes
- clear names
- type hints
- simple functions
- reusable utilities
- explicit errors
- deterministic behavior

Avoid:

- large rewrites
- speculative abstractions
- new dependencies unless requested
- hidden global state
- duplicate logic
- magic numbers
- changing public APIs without explicit approval

---

## Verification

Before saying a task is complete, run relevant checks whenever possible:

- tests
- lint
- type checks
- build
- smoke test

If a command cannot be run, say why.

Never say "fixed" or "done" unless verification has been completed or the limitation is clearly stated.

---

## AI/ML Rules

Before modifying AI/ML code, verify:

- tensor shapes
- dtype
- device
- batch dimension
- dataset split
- random seed
- loss function compatibility
- metric definition
- training/evaluation mode

Never tune on the test set.
Never leak future information.
Never fabricate metrics.
Never compare experiments with different evaluation protocols.

Read `docs/AI_RULES.md` before ML changes.

---

## Research Rules

Never fabricate:

- citations
- DOI
- page numbers
- benchmark results
- ablation results
- hyperparameters
- paper claims

Always distinguish:

- what the paper says
- what the implementation does
- what we observed
- what is future work

Read `docs/PAPER_WRITING.md` for research or paper-writing tasks.

---

## Project Documents

Use these files when relevant:

- `docs/ARCHITECTURE.md` for structure and design changes
- `docs/CODING_STYLE.md` for implementation style
- `docs/AI_RULES.md` for ML and AI work
- `docs/TESTING.md` before completion
- `docs/EXPERIMENTS.md` for experiment tracking
- `docs/DATASETS.md` before using data
- `docs/NOTEBOOK_RULES.md` for notebooks
- `docs/PAPER_WRITING.md` for papers and reports
- `docs/DECISIONS.md` for architecture decisions

---

## Final Response Format

When finishing a task, summarize:

1. What changed
2. Files changed
3. Commands run
4. What passed
5. What failed or was not run
6. Risks or uncertainties
