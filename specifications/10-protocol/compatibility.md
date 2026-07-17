# Compatibility

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

Compatibility rules define what the protocol must preserve across versions and implementations.

## Objective

State the contract expectations that protect interoperability.

## Scope

This document covers compatibility behavior only.

## Diagram

```mermaid
flowchart LR
  Old["Older version"] --> Compat["Compatibility rules"]
  Compat --> New["Newer version"]
```

## Responsibilities

- Preserve interoperable behavior where possible.
- Define the conditions for safe evolution.
- Help SDKs and servers coordinate change.

## Non-Responsibilities

- Guarantee unlimited backward support.
- Replace release policy.
- Hide breaking changes.

## Notes

Compatibility should be treated as a design constraint, not an afterthought.

## References

- [versioning.md](versioning.md)
- [states.md](states.md)
- [../15-release/release-policy.md](../15-release/release-policy.md)

## Acceptance Criteria

- Compatibility expectations are explicit.
- The document supports practical evolution.
- The rules are easy to reference.
