# ADR 0002: Engine Integration Belongs in SDKs

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

Resonance needs first-class integrations for several runtimes, but each runtime has its own APIs, packaging rules, and developer expectations.
Mixing those concerns into the core would make the foundation harder to maintain and harder to reuse.

## Decision

All engine-specific integration logic will live in `sdk/`.

- `sdk/` may contain language bindings, engine adapters, and runtime-specific convenience layers.
- `sdk/` may depend on engine APIs.
- `sdk/` must preserve the semantics of the core instead of redefining them.
- SDKs are separate products of the repository, not a convenience shortcut around the core boundary.

## Consequences

- Each engine can evolve at its own pace.
- SDK maintainers can ship integrations without changing the core architecture.
- The repository can host multiple integration strategies side by side.
- Documentation must clearly distinguish core concepts from adapter-specific behavior.

## Notes

This decision supports the planned layout described in `sdk/README.md` and `architecture/sdk.md`.
