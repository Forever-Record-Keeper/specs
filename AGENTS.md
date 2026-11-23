# Instructions for agents in the specs repo

This repo contains the plans for Forever Record Keeper. It contains no product code.

## Rules

- Write in plain English and US spelling.
  The rules are in the contributing guide of the `.github` repo.
- Run `vale .` before each commit. It must report no errors.
- Commit messages and PR titles follow Conventional Commits.
- Don't commit to `main`. Open a PR for every change.
- Don't copy text from a source without a license that allows it.
  Record each new source in `PROVENANCE.md`.
- Use the terms of `glossary.md`. Add a new term there before you use it.
- Record each new decision in `decisions/`, in the format of `decisions/README.md`.
  Never change the decision of an accepted record. Write a new record that replaces it.

## Review

The maintainer reviews requirements, scenarios and decision records in person.
Make those PRs small and easy to read.
