# 0003. The specs repo is an OpenSpec store

Date: 2026-11-23

## Decision

The `specs` repo is an OpenSpec store with the name `forever-record-keeper`.
Each code repo points to the store: its `openspec/config.yaml` contains only the line `store: forever-record-keeper`.
Each machine registers the store once.
OpenSpec never clones, pulls or pushes the store.
The project pins the OpenSpec version.

## Reason

A change that touches several repos gets 1 plan.
OpenSpec has the store feature built in.

## Consequences

- Stores are a beta feature of OpenSpec.
  The project updates OpenSpec only through a change of the pinned version.
- OpenSpec does not route tasks to repos.
  A change lists its tasks for each repo, and the coordinator briefs each repo (see 0011).
- Each machine needs 1 setup step to register the store.
