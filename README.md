# Specs of Forever Record Keeper

This repo contains the plans for Forever Record Keeper.
It contains no product code.

The other repos of the project implement these plans.
The [repo list of the organization](https://github.com/orgs/Forever-Record-Keeper/repositories) shows them.

## How work flows

A change to behavior starts here, as a plan with requirements and scenarios.
The maintainer reviews the plan.
Then the code repos implement it, 1 repo at a time.
A small fix that stays in 1 repo skips this repo.

The [contributing guide](https://github.com/Forever-Record-Keeper/.github/blob/main/CONTRIBUTING.md) explains both ways in detail.

## The OpenSpec store

This repo is an [OpenSpec](https://github.com/Fission-AI/OpenSpec) store with the name `forever-record-keeper`.
OpenSpec stores are a beta feature.

- `openspec/specs/` holds the living specs, 1 folder for each capability.
- `openspec/changes/` holds the changes in progress, and `openspec/changes/archive/` the finished ones.
- `.openspec-store/store.yaml` gives the store its name.

Each code repo points to this store with 1 line in its `openspec/config.yaml`: `store: forever-record-keeper`.

### Set up your machine

You need Node.js 26 and the pnpm version in `package.json`.
Clone this repo next to the other repos of the project, then run these commands in it:

```bash
pnpm install
pnpm exec openspec store register . --id forever-record-keeper
```

OpenSpec sends anonymous usage data by default.
To turn this off, run `pnpm exec openspec config set telemetry.enabled false`, or set `OPENSPEC_TELEMETRY=0`.

## Checks

- Vale checks all text against the plain English rules of the project.
  Run `vale sync` once, then `vale .`.
- OpenSpec checks the structure of all specs and changes: `pnpm run validate`.

## Sources

[PROVENANCE.md](PROVENANCE.md) lists the sources of tools, formats and ideas, with their licenses.

## Decisions and terms

- [`decisions/`](decisions) holds the decision records. [decisions/README.md](decisions/README.md) explains their format.
- `glossary.md` lists the terms of the project, with 1 word for each concept.

## License

MIT, see [LICENSE](LICENSE).
