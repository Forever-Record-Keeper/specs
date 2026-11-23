# 0027. Strict `en_US` dictionary for spelling

- Status: accepted
- Date: 2026-11-23

## Decision

The FRK Vale package checks spelling with the SCOWL `en_US` dictionary (size 60).
The package turns off the built-in Vale dictionary.
A small `frk` dictionary adds ordinary technical words such as "repo".

## Reason

The built-in dictionary accepts British spellings such as `licence`.

## Consequences

- A correct technical word fails the check until the `frk` dictionary has the word.
- Names with a fixed spelling go into the vocabulary of names (see 0021).
