# 0015. US spelling

- Status: accepted
- Date: 2026-11-23

## Decision

Text in the project uses US spelling.
The FRK Vale package checks the spelling (see 0027).

## Reason

The spell check needs 1 variant of English.
The FRK Vale package uses a strict `en_US` dictionary.

## Consequences

- Authors write "license", "color" and "behavior".
- The check fails on British spellings.
