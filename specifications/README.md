# Specifications

## Index

- [Purpose](#purpose)
- [Document Map](#document-map)
- [Reading Order](#reading-order)
- [Governance](#governance)
- [Acceptance Criteria](#acceptance-criteria)

## Purpose

This directory contains the technical specification for Resonance.
It is the contract that future implementation work must follow.

## Document Map

- `01-product/` product intent, scope, and success criteria.
- `02-architecture/` system structure and dependency rules.
- `03-core/` core layer responsibilities and boundaries.
- `04-network/` behavior expected from networking concepts.
- `05-audio/` audio and voice pipeline expectations.
- `06-spatial/` spatial interaction and placement rules.
- `07-server/` server-side behavioral expectations.
- `08-sdk/` SDK goals, constraints, and integration flow.
- `09-api/` API philosophy and cross-cutting API rules.
- `10-protocol/` protocol concepts, states, and compatibility rules.
- `11-performance/` performance targets and budgets.
- `12-security/` trust, threat, and protection model.
- `13-testing/` test strategy and validation model.
- `14-build/` build matrix and environment expectations.
- `15-release/` release policy and support rules.
- `16-roadmap/` technical backlog and delivery phases.
- `17-rfc/` RFC process and change governance.
- `18-glossary/` shared terminology.

## Reading Order

1. Start with `01-product/` to understand intent.
2. Read `02-architecture/` to understand boundaries.
3. Read `03-core/` through `10-protocol/` before any implementation.
4. Use `11-performance/` through `18-glossary/` as cross-cutting reference.

## Governance

Specifications in this directory are authoritative for future implementation.
If a document conflicts with earlier drafts or notes, the specification wins.

## Acceptance Criteria

- Every planned concept has a documented home.
- Every major boundary has explicit responsibilities and exclusions.
- The repository can be implemented without inventing missing rules.
