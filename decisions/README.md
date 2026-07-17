# Architecture Decision Records

## Index

- [Purpose](#purpose)
- [How to Use ADRs](#how-to-use-adrs)
- [File Naming](#file-naming)

## Purpose

This directory stores Architecture Decision Records for Resonance.
ADRs provide a durable record of why a choice was made, not just what was chosen.

## How to Use ADRs

1. Create a new ADR when a decision has long-term architectural impact.
2. Write the context, decision, and consequences before implementation.
3. Reference the ADR from related documentation when the topic becomes important later.

## File Naming

Use a zero-padded numeric prefix followed by a short descriptive slug.
Examples:

- `0001-example-decision.md`
- `0002-another-decision.md`

## Current ADRs

- [0001: Core Must Remain Engine-Agnostic](0001-core-is-engine-agnostic.md)
- [0002: Engine Integration Belongs in SDKs](0002-sdks-own-engine-integration.md)
- [0003: Protocol Is a Separate Contract Layer](0003-protocol-is-a-separate-contract-layer.md)
- [0004: Server Is Optional and Separate](0004-server-is-optional-and-separate.md)
- [0005: Versioning and Pre-1.0 Policy](0005-versioning-and-pre-1-0-policy.md)
- [0006: KISS Is a Primary Design Rule](0006-kiss-is-a-primary-design-rule.md)
- [0007: Documentation and ADRs Govern Structural Change](0007-documentation-and-adrs-govern-structural-change.md)
- [0008: Monorepo With Separate Boundaries](0008-monorepo-with-separate-boundaries.md)
