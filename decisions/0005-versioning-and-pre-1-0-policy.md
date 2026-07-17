# ADR 0005: Versioning and Pre-1.0 Policy

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

The project is still in its foundation phase, but it must already have a predictable compatibility story.
Without an explicit policy, contributors may assume a level of stability that the repository is not yet ready to promise.

## Decision

Resonance will follow Semantic Versioning, with a clearly defined pre-1.0 interpretation.

- `0.x` is a foundation and stabilization series.
- Breaking changes may occur before `1.0`, but they must still be documented deliberately.
- Each release must explain its compatibility impact and the maturity of the affected surface.

## Consequences

- Contributors know that pre-1.0 releases are not a free-for-all; they still need justification and documentation.
- Release notes must be explicit about what is stable and what may still move.
- The project can move quickly during the foundation phase without pretending that all contracts are final.
- Future `1.0` readiness becomes a deliberate milestone instead of an accident.

## Notes

This decision is the policy basis for `VERSIONING.md` and `RELEASE_STRATEGY.md`.
