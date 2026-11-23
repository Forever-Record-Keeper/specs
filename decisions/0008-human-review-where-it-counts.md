# 0008. Human review where it counts

- Status: accepted
- Date: 2026-11-23

## Decision

The maintainer reviews requirements, scenarios and the layer rules of the code.
The maintainer also reviews the paths with special security needs.
Those paths are the LAN server, the communication between processes, file access and Warcraft Logs tokens.
The maintainer merges every PR.
Automated checks and agents check the rest.

## Reason

Strict limits on the code replace a human read of every line.
The idea comes from public posts and talks by Robert C. Martin.

<!-- vale FRK.Spelling = NO -->
A human still reviews security, as Grady Booch argues.
<!-- vale FRK.Spelling = YES -->

## Consequences

- The `CODEOWNERS` file of each repo marks the paths for human review.
- Every PR waits for the maintainer.
- The automated checks must be strict (see 0009).
