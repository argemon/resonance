# API Philosophy

## Index

- [Purpose](#purpose)
- [Design Principles](#design-principles)
- [Public Surface Rules](#public-surface-rules)
- [Documentation Expectations](#documentation-expectations)

## Purpose

Resonance APIs should be easy to understand, hard to misuse, and stable enough to support multiple engines over many years.

## Design Principles

- Prefer explicit contracts over implicit behavior.
- Keep APIs small and composable.
- Separate data modeling from runtime integration.
- Preserve engine neutrality at the core boundary.

## Public Surface Rules

- Public APIs should expose the minimum necessary concepts.
- Names should describe intent, not implementation detail.
- Cross-cutting policy should live in shared documentation, not hidden conventions.

## Documentation Expectations

- Every public concept should have a clear description.
- Breaking changes should be explained before they are shipped.
- API decisions with lasting impact should be captured in ADRs.
