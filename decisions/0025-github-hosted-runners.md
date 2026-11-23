# 0025. GitHub-hosted runners

- Status: accepted
- Date: 2026-11-24

## Decision

CI runs on GitHub-hosted runners.
The project runs no self-hosted runners.

## Reason

GitHub-hosted runners are free for public repos.
GitHub recommends against self-hosted runners for public repos.
A PR from a fork can run code on a self-hosted runner.

## Consequences

- CI uses the machines and the limits that GitHub offers.
