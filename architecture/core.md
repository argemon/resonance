# Core Architecture

## Index

- [Responsibility](#responsibility)
- [Boundaries](#boundaries)
- [Expected Shape](#expected-shape)

## Responsibility

The core is the stable, engine-neutral boundary of Resonance.
It should define concepts and relationships without embedding runtime, engine, or transport assumptions.

## Boundaries

- No direct dependency on Unity, Unreal, Godot, or any other engine.
- No server ownership.
- No protocol implementation detail beyond contract intent.

## Expected Shape

The core should remain small, explicit, and easy to reason about.
Anything that varies by engine or deployment environment belongs outside the core.
