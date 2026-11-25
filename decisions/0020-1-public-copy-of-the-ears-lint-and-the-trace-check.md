# 0020. 1 public copy of the EARS lint and the trace check

Date: 2026-11-23

## Decision

The EARS lint and the trace check exist once, in the public `.github` repo.
The agent tooling calls the public checks and has no copy of them.

## Reason

2 copies of a check stop matching over time.
CI may depend only on public repos (see 0007).

## Consequences

- A fix to a check goes into 1 place.
- The agent tooling depends on the `.github` repo.
