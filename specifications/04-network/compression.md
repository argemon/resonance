# Compression

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

Compression is an optional behavior used to reduce bandwidth or storage cost when it is beneficial.

## Objective

Define the expected role of compression without requiring a specific algorithm.

## Scope

This document covers compression policy, not implementation.

## Diagram

```mermaid
flowchart LR
  Data["Data"] --> MaybeCompress["Optional compression"]
  MaybeCompress --> Transport["Transport"]
```

## Responsibilities

- Reduce bandwidth where appropriate.
- Preserve data integrity.
- Remain optional and policy-driven.

## Non-Responsibilities

- Force compression everywhere.
- Define algorithm choice.
- Hide costs from performance planning.

## Notes

Compression should be used only when it supports the performance budget.

## References

- [packet.md](packet.md)
- [../11-performance/targets.md](../11-performance/targets.md)
- [../12-security/security-model.md](../12-security/security-model.md)

## Acceptance Criteria

- Compression is optional.
- Integrity expectations are clear.
- Performance impact is documented.
