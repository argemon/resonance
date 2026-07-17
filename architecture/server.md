# Server Architecture

## Index

- [Purpose](#purpose)
- [Relationship to Core](#relationship-to-core)
- [Constraints](#constraints)

## Purpose

The server layer is reserved for future service-side components that support Resonance deployments.

## Relationship to Core

Server functionality must consume the core contract rather than define it.
This keeps the server optional and avoids making the project server-first.

## Constraints

- Do not place engine-specific logic here.
- Do not let server concerns leak into the core contract.
- Keep the server conceptually separate from protocol ownership.
