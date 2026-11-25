# 0028. Shared tooling as an npm package

Date: 2026-11-24

## Decision

The shared checks and configurations for TypeScript are the npm package `@forever-record-keeper/tooling`.
The source of the package is in the `.github` repo.
A workflow in the `.github` repo stages each release on npm with trusted publishing.
The maintainer approves each staged release on npm before it goes live.

## Reason

Each repo pins a version of the package and updates it with a PR.
Trusted publishing needs no npm token in the repo or in GitHub.
The approval step keeps each release under the review of the maintainer.

## Consequences

- The maintainer creates the npm organization `forever-record-keeper` and publishes the first version from a local clone.
- A repo gets a change to a check after a release and an update PR in that repo.
- The EARS lint and the trace check of 0020 are part of this package.