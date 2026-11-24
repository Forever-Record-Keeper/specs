# 0005. Requirements use EARS

Date: 2026-11-23

## Decision

Each requirement is 1 sentence of 20 words or fewer.
The sentence follows an EARS pattern and uses the keyword `SHALL`.
The patterns cover a rule that always applies, an event ("When"), a state ("While"), unwanted behavior ("If ... then") and an optional feature ("Where").
A lint checks the form.

## Reason

EARS gives clear requirements that a test can check.
Readers who are not native speakers can follow them.

<!-- vale FRK.Spelling = NO -->
The source is Mavin et al., "Easy Approach to Requirements Syntax", IEEE RE 2009.
<!-- vale FRK.Spelling = YES -->

## Consequences

- Detail that does not fit in 20 words moves into a scenario.
- Authors learn 5 patterns.
- The lint exists once, in a public repo (see 0020).
