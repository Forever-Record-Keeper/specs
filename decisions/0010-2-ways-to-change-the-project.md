# 0010. 2 ways to change the project

- Status: accepted
- Date: 2026-11-23

## Decision

Work of feature size is a change, and it may touch several repos.
Each change goes through an OpenSpec change in `specs`.
Small work in 1 repo is a fix.
The fix goes straight to an issue and a PR in that repo.
CI runs the same checks in both cases.

## Reason

The process matches the size of the work.

## Consequences

- A fix needs no OpenSpec change and no review of a plan.
- A change waits for the maintainer to review its plan.
