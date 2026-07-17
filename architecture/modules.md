# Modules Architecture

## Index

- [Module Map](#module-map)
- [Dependency Direction](#dependency-direction)

## Module Map

- `foundation/` documents the product intent.
- `architecture/` documents the structure.
- `decisions/` documents long-term choices.
- `core/` defines the central abstraction boundary.
- `protocol/` holds future contract definitions.
- `server/` hosts optional service-side logic.
- `sdk/` contains integration layers for external runtimes.
- `examples/`, `benchmarks/`, and `tests/` support validation and adoption.

## Dependency Direction

Dependencies should flow outward from the core domain to adapters, not the other way around.
This keeps the most stable concepts closest to the center and the most volatile integrations at the edge.
