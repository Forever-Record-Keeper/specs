# 0004. Executable scenarios live in code

- Status: accepted
- Date: 2026-11-23

## Decision

Each OpenSpec scenario has an ID, for example `REC-01`.
The code repo that implements the scenario contains the Gherkin scenario that tests it.
The Gherkin scenario has the ID as a tag, for example `@REC-01`.
A trace check matches the IDs in `specs` with the tags in the code repos.

## Reason

Specs are plans with a short life.
Tests stay with the code and describe what the code does today.

## Consequences

- A scenario ID stays the same once a test uses it.
- A reader finds the test for a scenario through its tag.
- The trace check exists once, in a public repo (see 0020).
