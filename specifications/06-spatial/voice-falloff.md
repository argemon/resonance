# Voice Falloff

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

Voice falloff defines how voice intensity changes with spatial conditions.

## Objective

Describe the expected audible behavior at different distances or conditions.

## Scope

This document covers falloff semantics only.

## Diagram

```mermaid
flowchart LR
  Voice["Voice"] --> Distance["Distance"]
  Distance --> Falloff["Falloff behavior"]
```

## Responsibilities

- Describe audible attenuation expectations.
- Support consistent spatial perception.
- Work with spatial zones and environment rules.

## Non-Responsibilities

- Define the exact attenuation curve.
- Replace occlusion behavior.
- Choose engine-specific audio routing.

## Notes

Falloff should be understandable and predictable before it is configurable.

## References

- [distance-models.md](distance-models.md)
- [directional-audio.md](directional-audio.md)
- [../05-audio/latency-targets.md](../05-audio/latency-targets.md)

## Acceptance Criteria

- Falloff behavior is explicit.
- The model is compatible with multiple engines.
- The document does not define implementation math.
