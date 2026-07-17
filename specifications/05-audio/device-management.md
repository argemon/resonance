# Device Management

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

Device management covers discovery, selection, availability, and change handling for audio devices.

## Objective

Specify device behavior in a platform-neutral way.

## Scope

This document covers device lifecycle expectations only.

## Diagram

```mermaid
flowchart LR
  Discover["Discover"] --> Select["Select"]
  Select --> Monitor["Monitor"]
  Monitor --> Switch["Switch"]
```

## Responsibilities

- Support device discovery and selection.
- Handle device availability changes gracefully.
- Keep the model portable across runtimes.

## Non-Responsibilities

- Implement device drivers.
- Expose OS-specific quirks as core behavior.
- Overcomplicate selection policy.

## Notes

Device management should be predictable and robust, not feature-heavy.

## References

- [capture.md](capture.md)
- [playback.md](playback.md)
- [../14-build/build-matrix.md](../14-build/build-matrix.md)

## Acceptance Criteria

- Device lifecycle is explicit.
- Changes are handled gracefully.
- The document remains implementation-neutral.
