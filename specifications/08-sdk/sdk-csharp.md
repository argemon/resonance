# SDK C#

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

The C# SDK provides a managed integration surface for engines and applications that use the .NET ecosystem.

## Objective

Define the role and boundaries of the C# SDK.

## Scope

This document covers the C# adapter concept and integration intent.

## Diagram

```mermaid
flowchart LR
  Core["Core"] --> CSharp["SDK C#"]
  CSharp --> Apps["Managed apps and tools"]
```

## Responsibilities

- Provide idiomatic managed integration.
- Preserve core semantics.
- Support downstream engine adapters where useful.

## Non-Responsibilities

- Depend on a specific engine.
- Introduce implementation that belongs in native core.
- Replace the C SDK where native integration is needed.

## Notes

The C# SDK should remain simple enough to integrate cleanly into multiple runtimes.

## References

- [sdk-c.md](sdk-c.md)
- [unity.md](unity.md)
- [../09-api/api-philosophy.md](../09-api/api-philosophy.md)

## Acceptance Criteria

- The C# SDK is clearly separate from the core.
- Managed APIs preserve core meaning.
- The design stays portable.
