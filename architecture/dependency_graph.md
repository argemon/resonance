# Dependency Graph

## Index

- [Target Direction](#target-direction)
- [Rules](#rules)

## Target Direction

```mermaid
flowchart LR
  Core["core"] --> Protocol["protocol"]
  Core --> SDK["sdk"]
  Protocol --> SDK
  SDK --> EngineA["engine/runtime A"]
  SDK --> EngineB["engine/runtime B"]
  Core --> Server["server"]
```

## Rules

- The core is the most stable layer.
- Protocol and SDK layers adapt, but do not redefine the core.
- Engines depend on SDKs, not on the core directly.
- Server-side components remain optional and separate.
