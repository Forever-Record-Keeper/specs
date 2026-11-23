# 0009. Strict checks from day one

- Status: accepted
- Date: 2026-11-23

## Decision

TypeScript code meets strict limits from the first commit.
Each function has a complexity of 6 or less, 25 lines or less, a nesting depth of 3 or less and 3 parameters or less.
Each file has 200 lines or less.
Coverage is 90% for lines and branches, the CRAP score stays under 10 and the mutation score on changed files is 85% or more.
The checks fail on a duplicate of 50 tokens or more, on unused code and on any Vale error.

## Reason

The repos start empty.
The limits apply without exceptions for old code.

## Consequences

- Each PR meets the limits before the merge.
- The code splits into many small functions and files.
- Mutation tests add CI time to each PR.
