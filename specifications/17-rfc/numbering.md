# RFC Numbering

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

RFC numbering defines how proposals are uniquely identified.

## Objective

Create a simple and durable numbering rule.

## Scope

This document covers RFC identifiers only.

## Diagram

```mermaid
flowchart LR
  Prefix["Zero-padded number"] --> Name["Descriptive slug"]
  Name --> Identifier["RFC identifier"]
```

## Responsibilities

- Provide unique identifiers.
- Keep RFC files sorted.
- Support stable references.

## Non-Responsibilities

- Encode status in the number.
- Replace title conventions.
- Introduce complex naming rules.

## Notes

Numbers should be assigned in order and never reused.

## References

- [rfc-template.md](rfc-template.md)
- [rfc-process.md](rfc-process.md)
- [states.md](states.md)

## Acceptance Criteria

- Numbering is deterministic.
- References stay stable.
- The rule remains easy to follow.
