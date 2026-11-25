# Instructions for agents in the specs repo

This repo contains the plans for Forever Record Keeper. It contains no product code.

## Rules

- Write in plain English and US spelling.
  The rules are in the contributing guide of the `.github` repo.
- Run `vale .` and `pnpm run validate` before each commit. Both must report no errors.
- Set `OPENSPEC_TELEMETRY=0` for every OpenSpec command.
- `openspec/config.yaml` holds the rules for proposals, specs and tasks. Follow them.
- Commit messages and PR titles follow Conventional Commits.
- Don't commit to `main`. Open a PR for every change.
  Start each PR from `main` and target `main`, as decision 0031 explains.
- Don't copy text from a source without a license that allows it.
  Record each new source in `PROVENANCE.md`.
- Use the terms of `glossary.md`. Add a new term there before you use it.
- Record each new decision in `decisions/`, in the format of `decisions/README.md`.
  To change a decision, edit its record and add a line to its Changes part.
  Don't write a second record on the same topic.

## Review

The maintainer reviews requirements, scenarios and decision records in person.
Make those PRs small and easy to read.
