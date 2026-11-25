# 0031. PRs start from main

Date: 2026-11-25

## Decision

Each PR starts from `main` and targets `main`.
A PR that needs the changes of an open PR waits for its merge.
When the wait costs too much, both become stacked PRs on GitHub.
Outside a stack, a PR never targets the branch of another PR.
The folder of the decision records has no index.

## Reason

Each PR then shows only its own changes.
A squash merge gives the changes of a PR a new commit.
A PR on the branch of a merged PR then shows the changes of both, until someone moves it onto `main` by hand.
The merge of such a PR goes into the other branch and doesn't reach `main`.
GitHub merges stacked PRs into `main`, and it moves the rest of the stack after each merge.
Each new record would add a row at the end of the index, so 2 open PRs with records would always conflict.

## Consequences

- Work that needs an open PR waits for its merge or goes into a stack.
- A PR that conflicts with a newer `main` moves onto `main` before its merge.
- The file name of each record starts with its number.
  The folder view of GitHub then lists the records in order.
