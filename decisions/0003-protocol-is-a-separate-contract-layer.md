# ADR 0003: Protocol Is a Separate Contract Layer

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

The project needs a clear place for public contracts that are stable enough to be shared across engines and deployment styles.
Those contracts should not be confused with a server implementation, and they should not be buried inside an SDK.

## Decision

`protocol/` will be the dedicated home for public contract documentation and contract-oriented design.

- It will define the shape of the public contract surface.
- It will remain separate from `server/` and `sdk/`.
- It will describe intent and compatibility expectations, not runtime implementation details.

## Consequences

- The protocol can evolve independently from any one server or SDK implementation.
- Public contract changes will be easier to review because they are isolated in one place.
- Implementation teams get a clearer source of truth for interoperability decisions.
- The repository avoids mixing specification, transport, and runtime concerns.

## Notes

This decision aligns with the architectural separation described in `architecture/modules.md` and `architecture/dependency_graph.md`.
