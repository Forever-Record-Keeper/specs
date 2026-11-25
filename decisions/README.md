# Decision records

A decision record states 1 decision of the project and the reason for it.
The project numbers the records from 0001 on and keeps them in this folder.
To change a decision, a PR edits its record (see 0030).
To drop a decision, a PR deletes its record.
The project doesn't use the number of a deleted record again.
Git keeps the earlier versions.

## Format

Each record has these parts:

- A title line with the number and the title.
- A line with the date of the decision.
- Decision: what the project does.
- Reason: why the project does it.
- Consequences: what follows from the decision, with the costs.
- Changes: 1 line for each change of the decision, with the date, the PR and the reason.
  A record gets this part with its first change.

## Index

| Number | Title | Date |
| --- | --- | --- |
| [0001](0001-separate-repos.md) | Separate repos | 2026-11-23 |
| [0002](0002-sibling-clones-no-git-submodules.md) | Sibling clones, no git submodules | 2026-11-23 |
| [0003](0003-the-specs-repo-is-an-openspec-store.md) | The specs repo is an OpenSpec store | 2026-11-23 |
| [0004](0004-executable-scenarios-live-in-code.md) | Executable scenarios live in code | 2026-11-23 |
| [0005](0005-requirements-use-ears.md) | Requirements use EARS | 2026-11-23 |
| [0006](0006-plain-us-english.md) | Plain US English | 2026-11-23 |
| [0007](0007-agent-tooling-in-a-separate-repo.md) | Agent tooling in a separate repo | 2026-11-23 |
| [0008](0008-human-review-where-it-counts.md) | Human review where it counts | 2026-11-23 |
| [0009](0009-strict-checks-from-day-one.md) | Strict checks from day one | 2026-11-23 |
| [0010](0010-2-ways-to-change-the-project.md) | 2 ways to change the project | 2026-11-23 |
| [0011](0011-coordinator-and-worker-sessions.md) | Coordinator and worker sessions | 2026-11-23 |
| [0012](0012-agents-md-is-the-instruction-file.md) | `AGENTS.md` is the instruction file | 2026-11-23 |
| [0013](0013-mit-license-for-every-repo.md) | MIT License for every repo | 2026-11-23 |
| [0014](0014-website-address.md) | Website address | 2026-11-23 |
| [0015](0015-us-spelling.md) | US spelling | 2026-11-23 |
| [0016](0016-nodejs-26-and-pnpm.md) | Node.js 26 and pnpm | 2026-11-23 |
| [0017](0017-conventional-commits-for-commit-messages-and-pr-titles.md) | Conventional Commits for commit messages and PR titles | 2026-11-23 |
| [0018](0018-no-sign-off-for-now.md) | No sign-off for now | 2026-11-23 |
| [0019](0019-agents-open-prs-with-their-own-identity.md) | Agents open PRs with their own identity | 2026-11-23 |
| [0020](0020-1-public-copy-of-the-ears-lint-and-the-trace-check.md) | 1 public copy of the EARS lint and the trace check | 2026-11-23 |
| [0021](0021-2-vale-vocabularies.md) | 2 Vale vocabularies | 2026-11-23 |
| [0022](0022-contributor-covenant-2-1-as-the-code-of-conduct.md) | Contributor Covenant 2.1 as the code of conduct | 2026-11-23 |
| [0023](0023-private-security-reports.md) | Private security reports | 2026-11-23 |
| [0024](0024-only-collaborators-open-prs-for-now.md) | Only collaborators open PRs for now | 2026-11-23 |
| [0025](0025-github-hosted-runners.md) | GitHub-hosted runners | 2026-11-24 |
| [0026](0026-starlight-for-the-docs.md) | Starlight for the docs | 2026-11-24 |
| [0027](0027-strict-en-us-dictionary-for-spelling.md) | Strict `en_US` dictionary for spelling | 2026-11-23 |
| [0028](0028-shared-tooling-as-an-npm-package.md) | Shared tooling as an npm package | 2026-11-24 |
| [0029](0029-typescript-6-0-for-now.md) | TypeScript 6.0 for now | 2026-11-24 |
| [0030](0030-decision-records-change-in-place.md) | Decision records change in place | 2026-11-24 |
