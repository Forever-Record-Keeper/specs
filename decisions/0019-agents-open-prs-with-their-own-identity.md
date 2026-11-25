# 0019. Agents open PRs with their own identity

Date: 2026-11-23

## Decision

Agents open PRs through a GitHub App or a second account.
The maintainer reviews and merges each PR.

## Reason

GitHub doesn't let the author of a PR approve it.
Required code owner reviews need an author other than the code owner.

## Consequences

- The project manages 1 more identity and its access.
- The maintainer approves agent PRs as the code owner.
