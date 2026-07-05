# AGENTS.md

Cross-agent instructions for Claude Code, Codex, Cursor, Gemini CLI, and other AI coding agents.

## Core Loop

Plan → Inspect → Implement → Verify → Review

Do not implement before inspecting the repository.

## Agent Behavior

Agents must:

- read existing code before writing
- avoid hallucinating interfaces
- follow local conventions
- minimize diffs
- preserve public behavior unless asked to change it
- explain uncertainty
- verify outputs

## Required Completion Summary

Every completed task should include:

- files changed
- assumptions made
- validation performed
- risks
- remaining follow-up work

## Escalation

If required context is missing, do not invent it.

Instead:

1. state what is missing
2. identify where it should come from
3. make the safest minimal change only if appropriate
