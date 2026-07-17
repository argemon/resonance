# Project Scope

## Index

- [In Scope](#in-scope)
- [Out of Scope](#out-of-scope)
- [Boundary Rules](#boundary-rules)

## In Scope

- Foundation documents and governance.
- Engine-agnostic core boundaries.
- SDK planning and integration surfaces.
- Architecture decision records.
- Build, test, release, and contribution scaffolding.

## Out of Scope

- Runtime audio implementation.
- Runtime networking implementation.
- Server implementation.
- Engine-specific feature delivery in the core.

## Boundary Rules

Any feature that requires engine APIs must live outside the core and inside an SDK or integration layer.
