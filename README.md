# AI Engineering OS

**AI Engineering OS** is a practical operating system for Claude Code and AI coding agents.

It is designed to help AI agents:

- read before writing
- avoid hallucinated APIs and schemas
- follow existing codebase patterns
- verify work before claiming success
- support AI/ML research, PyTorch experiments, papers, and production engineering

## Quick Start

Copy the root files and `docs/` folder into your project:

```bash
cp CLAUDE.md AGENTS.md /path/to/project/
cp -r docs /path/to/project/
```

Then ask Claude Code:

```text
Read CLAUDE.md first, then follow the relevant docs for this task.
```

## Structure

```text
.
├── CLAUDE.md
├── AGENTS.md
└── docs/
    ├── AI_RULES.md
    ├── ARCHITECTURE.md
    ├── CODING_STYLE.md
    ├── DATASETS.md
    ├── DECISIONS.md
    ├── EXPERIMENTS.md
    ├── NOTEBOOK_RULES.md
    ├── PAPER_WRITING.md
    └── TESTING.md
```

## Goal

This project will grow into a full AI engineering handbook with standards, playbooks, checklists, examples, and anti-hallucination rules for coding agents.
