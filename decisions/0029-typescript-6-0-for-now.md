# 0029. TypeScript 6.0 for now

Date: 2026-11-24

## Decision

The TypeScript repos use TypeScript 6.0.
A later record moves them to TypeScript 7.

## Reason

The type-checked lint rules of 0009 come from `typescript-eslint`.
`typescript-eslint` 8 supports TypeScript up to version 6.0.
The tooling package, with its shared base configuration, also passes the type check of TypeScript 7.

## Consequences

- The repos miss the faster type check of TypeScript 7 for now.
- The move to TypeScript 7 needs a new version of the tooling package and a PR in each TypeScript repo.