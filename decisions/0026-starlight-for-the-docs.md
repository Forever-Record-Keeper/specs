# 0026. Starlight for the docs

- Status: accepted
- Date: 2026-11-24

## Decision

The docs site uses Starlight, the docs framework of the Astro project.
The project pins the Starlight version.

## Reason

Starlight uses the same TypeScript tools and the same base (Astro) as the planned website.
Starlight has a search that needs no external service (`Pagefind`).
Starlight has built-in support for English and German.
The pages are Markdown files that Vale checks.

## Consequences

- Until Starlight reaches version 1.0, an update may break the docs site.
- Pinned versions and update PRs handle such breaks.
- The docs site and the website share the same base.
