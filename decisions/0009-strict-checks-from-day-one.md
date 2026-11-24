# 0009. Strict checks from day one

- Status: accepted
- Date: 2026-11-23

## Decision

TypeScript code meets strict limits from the first commit.
Each function has a complexity of 6 or less and 25 lines of code or less.
The nesting depth of a function is 3 or less, and it has 3 parameters or less.
Each file has 200 lines of code or less.
Blank lines and comments don't count as lines of code.
Coverage is 90% for lines and branches, the CRAP score stays under 10 and the mutation score on changed files is 85% or more.
The checks fail on a duplicate of 50 tokens or more, on unused code and on any Vale error.

Each test is in a `describe` section, and each section and each test has a short title.
Sections nest 2 levels deep at most.
A test file has 500 lines of code or less.
Each test keeps the function limit, and the callback of a section has no function limit.

## Reason

The repos start empty.
The limits apply without exceptions for old code.
Sections with short titles make a test file read as a list of behaviors.
The callback of a section contains many tests and can't keep the function limit.
Test files need more room than source files for the sections of 1 unit.

## Consequences

- Each PR meets the limits before the merge.
- The code splits into many small functions and files.
- Mutation tests add CI time to each PR.
- The tooling package has its own function length rule, because the rule of ESLint can't skip the callback of a section.

## Changes

- 2026-11-24, [PR 6](https://github.com/Forever-Record-Keeper/specs/pull/6): adds the rules for test files and counts only lines of code.
  A test file then reads as a list of behaviors.
