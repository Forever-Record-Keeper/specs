# 0006. Plain US English

- Status: accepted
- Date: 2026-11-23

## Decision

All text that people read follows the plain English rules of the contributing guide.
Vale checks the text in 3 places: an agent hook, a pre-commit hook and CI.

## Reason

Most readers are not native speakers of English.
AI agents repeat the same patterns of phrasing again and again.

## Consequences

- A contributor sees a Vale error before the commit and again in CI.
- The FRK Vale package in the `.github` repo holds the rules for all repos.
- Authors spend more time on each text.
