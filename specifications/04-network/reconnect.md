# Reconnect

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

Reconnect behavior describes how a disconnected participant returns without losing unnecessary logical state.

## Objective

Describe reconnect expectations in a portable way.

## Scope

This document covers reconnect semantics, not transport retry algorithms.

## Diagram

```mermaid
flowchart LR
  Disconnect["Disconnect"] --> Retry["Retry path"]
  Retry --> Rejoin["Rejoin state"]
```

## Responsibilities

- Define how recovery should behave.
- Protect session continuity where possible.
- Support graceful recovery after transient failures.

## Non-Responsibilities

- Guarantee success.
- Choose retry policy implementation.
- Override security rules.

## Notes

Reconnect should restore only what is valid to restore.

## References

- [session.md](session.md)
- [heartbeat.md](heartbeat.md)
- [../07-server/player-lifecycle.md](../07-server/player-lifecycle.md)

## Acceptance Criteria

- Reconnect expectations are explicit.
- Recovery limits are clear.
- The document avoids transport assumptions.
