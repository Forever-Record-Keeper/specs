# 0030. Decision records change in place

- Status: accepted
- Date: 2026-11-24

## Decision

To change a decision, a PR edits its record.
The record keeps its number and gets a line in its Changes part, with the date, the PR and the reason.
To drop a decision, a PR deletes its record.
The project doesn't use the number of a deleted record again.
Git keeps the earlier versions of each record.

## Reason

Each topic has 1 record, and that record states the current decision.
Agents read only current decisions, so an old decision can't mislead them.
The diff of a PR shows the exact change.
The maintainer then reviews only what changed.
A copy of a decision in a second record drifts from the first.

## Consequences

- A reference such as "decision 0009" always points to the current decision on its topic.
- The earlier reasons are in the git history and in the PRs, not in the folder.
- When an earlier option matters for later choices, the reason of the record names it in 1 sentence.
