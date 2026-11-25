# 0002. Sibling clones, no git submodules

Date: 2026-11-23

## Decision

A contributor clones all available repos side by side in the same folder.
Scripts and settings find the other repos through relative paths such as `../specs`.
The project uses no git submodules.

## Reason

Sibling clones are simple to sync.
Each repo has its own history and its own CI.

## Consequences

- The relative paths work only when the repos share the same parent folder.
- No commit records which versions of the repos belong together.
