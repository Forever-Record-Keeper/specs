# 0007. Agent tooling in a separate repo

Date: 2026-11-23

## Decision

A private repo of the maintainer contains the agent tooling, a set of Claude Code plugins.
Each FRK repo works without the tooling.
Everything that CI checks is in public FRK repos.
A contributor without the tooling can build, test and pass CI.
The tooling may become public later under the MIT License.

## Reason

The ownership of the tooling is clear.
Other projects can use the tooling too.

## Consequences

- Each check that CI needs goes into a public FRK repo (see 0020).
- Agents and humans pass the same checks.
