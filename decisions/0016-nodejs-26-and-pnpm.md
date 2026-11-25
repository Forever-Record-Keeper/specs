# 0016. Node.js 26 and pnpm

Date: 2026-11-23

## Decision

Tools and code use Node.js 26 and pnpm.
Node.js 26 is the current LTS line.
Each repo pins its pnpm version in `package.json`.

## Reason

The TypeScript repos share the same set of tools.
An LTS line gets long support.

## Consequences

- A contributor installs Node.js 26 and the pnpm version of the repo.
- A move to a new Node.js line needs a PR in each TypeScript repo.
