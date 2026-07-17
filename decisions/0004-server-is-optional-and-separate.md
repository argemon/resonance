# ADR 0004: Server Is Optional and Separate

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

Resonance is a spatial interaction engine, not a server product in itself.
Even if the ecosystem eventually includes server-side components, those components should not define the core model or force server-first assumptions into the foundation.

## Decision

`server/` will remain an optional and isolated layer.

- Server-side components may be added later as separate concerns.
- The server layer must consume the core contract rather than define it.
- The core must not depend on server deployment details.

## Consequences

- The project can support both hosted and embedded deployment models later.
- The repository does not become biased toward a central server architecture.
- Core and SDK work can proceed independently of service-side implementation.
- Documentation must keep server concepts clearly separated from domain concepts.

## Notes

This decision is reflected in `architecture/server.md` and the current repository layout.
