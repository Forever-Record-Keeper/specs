# 0001. Separate repos

Date: 2026-11-23

## Decision

The project keeps its parts in separate repos of the GitHub organization `Forever-Record-Keeper`.
The specs and the docs have repos of their own too.
The [repo list of the organization](https://github.com/orgs/Forever-Record-Keeper/repositories) shows the current repos.

## Reason

Each repo is small and has its own rules.
The maintainer chose the split.

## Consequences

- A change can touch several repos and needs 1 plan for all of them (see 0003).
- The repos need a shared folder layout on each machine (see 0002).
- Each repo has its own CI, hooks and settings.
