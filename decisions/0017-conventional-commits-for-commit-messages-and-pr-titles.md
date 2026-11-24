# 0017. Conventional Commits for commit messages and PR titles

Date: 2026-11-23

## Decision

Commit messages and PR titles follow Conventional Commits.
The tool commitlint checks the form, and Vale checks the message body.
The project merges with squash merge.
The PR title becomes the commit message.

## Reason

The history is easy to read.
The commit messages give a base for release notes.

## Consequences

- The `main` branch gets 1 commit for each PR.
- A PR title must follow Conventional Commits before the merge.
