# Interest Management

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

Interest management determines which entities or events are relevant to a participant.

## Objective

Specify the behavior of relevance filtering without prescribing a data structure.

## Scope

This document covers interest-based visibility and delivery semantics.

## Diagram

```mermaid
flowchart LR
  World["World state"] --> Filter["Interest filter"]
  Filter --> Recipient["Recipient"]
```

## Responsibilities

- Reduce unnecessary delivery.
- Support scalable proximity and relevance behavior.
- Keep relevance rules deterministic.

## Non-Responsibilities

- Choose spatial indexing.
- Define server replication internals.
- Force one global culling policy.

## Notes

Interest management is a relevance policy, not a feature bundle.

## References

- [latency.md](latency.md)
- [jitter.md](jitter.md)
- [../06-spatial/zones.md](../06-spatial/zones.md)

## Acceptance Criteria

- Relevance is clearly defined.
- The behavior supports scalability.
- The document remains implementation-neutral.
