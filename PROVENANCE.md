# Provenance

This file lists the sources that Forever Record Keeper uses: tools, formats, data and ideas.
Each entry states its license, and how the project uses it.
The project uses the MIT License, so each source must allow that use.

<!-- The tables list names of people, tools and packages, which no dictionary contains. -->
<!-- vale FRK.Spelling = NO -->

## Tools and packages

| Source | Use | License |
| --- | --- | --- |
| [OpenSpec](https://github.com/Fission-AI/OpenSpec) | Format and tool for specs and changes, with stores for planning in its own repo | MIT, used as a dependency |
| [Vale](https://vale.sh) | Prose checks | MIT, used as a tool |
| [`vale-ai-tells`](https://github.com/tbhb/vale-ai-tells) | Vale rules against common AI phrasing | MIT, used as a pinned package |
| [SCOWL en_US dictionary](https://github.com/wooorm/dictionaries) | US spelling check in the FRK Vale package | Permissive SCOWL license, kept in full beside the files in the `.github` repo |
| [Contributor Covenant 2.1](https://www.contributor-covenant.org/version/2/1/code_of_conduct/) | Code of conduct | CC BY 4.0, with its attribution kept |
| [actions/checkout](https://github.com/actions/checkout) | GitHub Actions step | MIT, used as a pinned action |

## Planned tools

The code repos will use these tools. Each one moves to the first table when a repo adds it.

| Source | Use | License |
| --- | --- | --- |
| Cucumber.js, ESLint, jscpd, dependency-cruiser | Checks for TypeScript code | MIT |
| Stryker | Mutation tests | Apache-2.0 |
| knip | Check for unused code | ISC |
| Starlight | Docs site | MIT |

## Formats and ideas

| Source | Use | Status |
| --- | --- | --- |
| [AGENTS.md](https://agents.md) | Format of the instruction file for agents | Open format |
| [Claude Code docs](https://code.claude.com/docs) | Hooks, subagents, plugins and settings | Ideas only |
| Mavin et al., "Easy Approach to Requirements Syntax", IEEE RE 2009 | EARS patterns for requirements | Published paper, ideas only |
| Savoia and Evans, 2007 | CRAP metric for the risk of a function | Published metric, ideas only |
| Robert C. Martin, public posts and talks of 2026 | Constraints instead of line-by-line review, and a sequence of review agents | Ideas only |
| [ub-mode](https://github.com/unclebob/ub-mode) | Inspiration | The repo has no license. The project copies nothing from it. |

## Not used

| Source | Reason |
| --- | --- |
| ASD-STE100 Simplified Technical English | Copyright and trademark of ASD. The project uses the general idea of a controlled language, and makes no claim to follow ASD-STE100. |
| Vale rules based on the Wikipedia page "Signs of AI writing" | CC BY-SA. The share-alike terms don't fit the MIT License. |
| Contributor Covenant 3.0 | CC BY-SA 4.0, a share-alike license. |

<!-- vale FRK.Spelling = YES -->
