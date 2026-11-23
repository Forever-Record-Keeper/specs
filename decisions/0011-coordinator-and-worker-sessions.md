# 0011. Coordinator and worker sessions

- Status: accepted
- Date: 2026-11-23

## Decision

The agent session that plans and coordinates a change runs in the `specs` repo.
Work in a code repo runs in a worker session.
The working folder of the worker session is that code repo.
The worker session has `specs` as an extra folder that it only reads.

## Reason

The `AGENTS.md` file, the hooks and the rules of a repo load only in a session that runs in that repo.

## Consequences

- The coordinator writes a brief for each repo of a change (see 0003).
- Each worker session follows the rules of its own repo.
