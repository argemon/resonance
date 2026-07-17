# Architecture

## Index

- [Overview](#overview)
- [Layering Model](#layering-model)
- [Boundaries](#boundaries)
- [Reference Documents](#reference-documents)

## Overview

Resonance is designed as an engine-agnostic spatial interaction foundation.
The architecture separates the durable domain core from optional integration surfaces so that
different engines can adopt the same conceptual model without sharing runtime dependencies.

## Layering Model

1. Foundation and governance define intent, scope, and change control.
2. Core documents describe the engine-neutral boundary.
3. Protocol documents will later describe stable external contracts.
4. SDKs adapt those contracts to specific engines and languages.
5. Server-side components, if any, remain isolated from the core model.

## Boundaries

- The core must not depend on any engine.
- SDKs may depend on engine APIs, but not the other way around.
- Documentation should describe concepts without implying implementation detail prematurely.

## Reference Documents

- `architecture/overview.md`
- `architecture/core.md`
- `architecture/server.md`
- `architecture/sdk.md`
- `architecture/modules.md`
- `architecture/dependency_graph.md`
- `architecture/future.md`
