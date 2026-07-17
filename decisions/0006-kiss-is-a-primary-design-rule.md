# ADR 0006: KISS Is a Primary Design Rule

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

Resonance is intended to last for many years and to be adopted across different engines and runtimes.
That kind of project can become over-engineered very quickly if every future possibility is modeled too early.

The foundation therefore needs an explicit rule that favors the simplest shape that satisfies the current need.

## Decision

KISS is a primary design rule for Resonance.

- Prefer the simplest architecture that cleanly solves the problem.
- Avoid speculative generalization.
- Avoid abstraction unless it reduces real duplication or real complexity.
- Prefer narrow, explicit contracts over flexible but unclear frameworks.

## Consequences

- The project stays easier to understand for new contributors.
- Future maintenance cost is lower because fewer moving parts exist.
- Some advanced ideas will be deferred until there is a concrete need for them.
- When complexity is introduced, it must be justified by actual requirements, not by anticipation.

## Notes

This decision applies to documentation, architecture, APIs, module boundaries, and future implementation work.
