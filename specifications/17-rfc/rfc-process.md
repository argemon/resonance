# RFC Process

## Index

- [Summary](#summary)
- [Objective](#objective)
- [Scope](#scope)
- [Diagram](#diagram)
- [Responsibilities](#responsibilities)
- [Non-Responsibilities](#non-responsibilities)
- [Notes](#notes)
- [References](#references)
- [Acceptance Criteria](#acceptance-criteria)

## Summary

The RFC process defines how a proposal moves from draft to decision.

## Objective

Describe the official path for proposing major changes.

## Scope

This document covers process flow only.

## Diagram

```mermaid
flowchart LR
  Idea["Idea"] --> Draft["Draft RFC"]
  Draft --> Review["Review"]
  Review --> Decision["Decision"]
```

## Responsibilities

- Define how to propose changes.
- Clarify review expectations.
- Make decisions traceable.

## Non-Responsibilities

- Replace everyday documentation updates.
- Create bureaucratic overhead.
- Duplicate ADR content.

## Notes

The process should be simple enough to use, but structured enough to protect the architecture.

## References

- [rfc-template.md](rfc-template.md)
- [states.md](states.md)
- [numbering.md](numbering.md)

## Acceptance Criteria

- The process is easy to follow.
- The stages are explicit.
- The workflow supports meaningful review.
