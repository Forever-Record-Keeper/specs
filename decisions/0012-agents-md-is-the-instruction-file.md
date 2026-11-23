# 0012. `AGENTS.md` is the instruction file

- Status: accepted
- Date: 2026-11-23

## Decision

Each repo has a short `AGENTS.md` file as the main instruction file for agents.
A `CLAUDE.md` file exists only where a tool needs one.
The `CLAUDE.md` file then only imports `AGENTS.md`.
Hooks and CI check the hard rules.

## Reason

`AGENTS.md` is an open format.
Agents follow a short file better than a long one.

## Consequences

- The instructions for agents have 1 source in each repo.
- Each hard rule needs a hook or a CI check.
