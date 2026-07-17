# ADR 0008: Monorepo With Separate Boundaries

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

Resonance needs to evolve as a shared ecosystem with core concepts, protocol work, SDKs, examples, tests, and future tooling.
Splitting those concerns too early into many repositories would make coordination harder and could obscure the dependency model.

At the same time, keeping everything in one place only works if boundaries remain explicit.

## Decision

Resonance will use a monorepo with clearly separated top-level directories for each major concern.

- Shared foundation, architecture, and decisions remain in the same repository.
- Core, protocol, server, SDKs, tests, benchmarks, and tooling are organized as separate top-level areas.
- Directory boundaries communicate ownership and dependency direction.

## Consequences

- Contributors can discover related work in one place.
- The repository can enforce architectural separation without introducing repo fragmentation.
- Automation, documentation, and future build tooling can operate against a single source of truth.
- The monorepo still requires discipline so that directories do not become accidental catch-all zones.

## Notes

This decision reflects the structure already defined in the repository layout and documented in `README.md`.
