# ADR 0001: Core Must Remain Engine-Agnostic

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

Resonance is intended to support Unity, Unreal, Godot, proprietary engines, simulators, and other 3D runtimes.
If the core layer depends on any engine, the project loses portability and the long-term maintenance cost rises sharply.

The core must therefore define only the stable domain boundary shared by every integration.

## Decision

The `core/` layer will remain strictly engine-agnostic.

- It may define shared concepts, policies, and data boundaries.
- It may not depend on engine APIs, engine build systems, or engine-specific runtime behavior.
- Any engine-facing behavior must live in a separate SDK or adapter layer.

## Consequences

- The project can support multiple engines without duplicating the core model.
- SDK authors can integrate Resonance without modifying core semantics.
- The architecture becomes easier to reason about because the center of the system remains stable.
- Some features that seem convenient in the short term must be deferred to adapters instead of being added directly to the core.

## Notes

This decision establishes the architectural constraint referenced by `architecture/core.md` and `architecture/overview.md`.
