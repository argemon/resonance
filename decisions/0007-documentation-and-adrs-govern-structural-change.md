# ADR 0007: Documentation and ADRs Govern Structural Change

## Index

- [Status](#status)
- [Context](#context)
- [Decision](#decision)
- [Consequences](#consequences)
- [Notes](#notes)

## Status

Accepted

## Context

The repository is foundation-first.
If structural changes are made without written context, the project will accumulate hidden assumptions that are difficult to review later.

Resonance needs a lightweight but durable way to preserve architectural intent.

## Decision

Documentation and ADRs are the default governance mechanism for structural change.

- Changes that affect boundaries, dependencies, compatibility, naming, or module ownership should be documented before implementation.
- ADRs should capture decisions with long-term architectural impact.
- Architecture documents should describe the current structural model.
- Foundation documents should describe scope, principles, and non-goals.

## Consequences

- Contributors have a clear place to explain why a change exists.
- Reviewers can assess tradeoffs before code is written.
- The project avoids relying on tribal knowledge for important decisions.
- Documentation maintenance becomes part of the project, not an afterthought.

## Notes

This decision complements `GOVERNANCE.md`, `decisions/README.md`, and the architecture documentation set.
