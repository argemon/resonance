# Resonance

Open Spatial Interaction Engine

## Index

- [Overview](#overview)
- [Motivation](#motivation)
- [Goals](#goals)
- [High-Level Architecture](#high-level-architecture)
- [Repository Organization](#repository-organization)
- [Roadmap](#roadmap)
- [How to Contribute](#how-to-contribute)
- [License](#license)
- [Project Status](#project-status)

## Overview

Resonance is an open source engine-agnostic foundation for spatial interaction in multiplayer applications.
It is intended to support voice, communication channels, proximity-driven events, and related interaction
primitives through separate SDKs rather than a hard dependency on any single engine.

This repository currently contains the project foundation only. No runtime implementation, networking stack,
audio pipeline, or protocol implementation is included at this stage.

## Motivation

Spatial communication is often rebuilt separately for every engine and game stack.
That repetition creates fragmentation, inconsistent APIs, and duplicated maintenance cost.
Resonance is being shaped as a shared foundation so teams can integrate the same conceptual model across
Unity, Unreal, Godot, proprietary engines, simulators, and other 3D applications.

## Goals

- Provide a clean, durable architectural foundation.
- Keep the core independent from any engine or platform SDK.
- Separate domain contracts from integration surfaces.
- Make the project easy to maintain for many years.
- Establish a professional open source workflow before implementation begins.

## High-Level Architecture

Resonance is organized around a layered model:

- `core/` defines the engine-agnostic domain boundary.
- `protocol/` will later describe public protocol contracts.
- `server/` will eventually host optional service-side components.
- `sdk/` contains integrations for specific runtimes and engines.
- `architecture/` and `foundation/` define the design intent and scope.

The core principle is strict separation of concerns. Engine-specific behavior belongs only in SDK layers.

## Repository Organization

- `.github/` GitHub workflows, templates, and repository automation.
- `docs/` supporting documentation hub.
- `foundation/` vision, mission, principles, scope, and use-case statements.
- `architecture/` architectural overviews and dependency documentation.
- `decisions/` architecture decision records.
- `protocol/` future protocol specification space.
- `core/` engine-agnostic core boundary.
- `server/` future server-side components.
- `sdk/` engine and language-specific SDK surfaces.
- `examples/` usage examples and reference applications.
- `benchmarks/` performance measurement scaffolding.
- `tests/` repository-level test strategy and future test assets.
- `scripts/` local project automation scripts.
- `tools/` internal tooling.
- `third_party/` dependency notes and external notices.
- `website/` public website and documentation site sources.

## Roadmap

The near-term roadmap is intentionally foundation-first:

1. Finalize governance and documentation baseline.
2. Define architectural boundaries and decision records.
3. Establish the public vocabulary for modules and APIs.
4. Prepare build, test, lint, and release scaffolding.
5. Begin implementation only after the foundation is complete.

## How to Contribute

Contributions should begin with architecture and documentation clarity.
Before implementing new behavior, confirm that the proposal fits the project scope, principles, and non-goals.
For significant changes, open an ADR in `decisions/` and align the design with maintainers before coding.

Please read `CONTRIBUTING.md`, `CODE_OF_CONDUCT.md`, and `SECURITY.md` before participating.

## License

Resonance is licensed under the MIT License. See `LICENSE` for the full text.

## Project Status

This project is in the foundation stage.
The repository is intentionally minimal and does not yet contain a production implementation.
Version `0.1` will focus on stable structure, shared terminology, and process readiness.
