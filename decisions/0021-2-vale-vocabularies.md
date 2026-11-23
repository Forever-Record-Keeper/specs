# 0021. 2 Vale vocabularies

- Status: accepted
- Date: 2026-11-23

## Decision

The FRK Vale package has a vocabulary of names, such as tools and products.
The glossary in `specs` is the source of project terms.
The release of the Vale package turns the glossary into a second vocabulary.

## Reason

Each kind of word has 1 owner.
Project terms have 1 source: the glossary.

## Consequences

- A new project term goes into the glossary first.
  The next release of the Vale package adds the term to the check.
- A new tool or product name goes into the vocabulary of names.
