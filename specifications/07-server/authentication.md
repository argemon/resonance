# Authentication

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

Authentication defines how the server verifies identity or trust claims.

## Objective

Specify the expected authentication behavior without selecting a scheme.

## Scope

This document covers authentication semantics only.

## Diagram

```mermaid
flowchart LR
  Claim["Identity claim"] --> Verify["Verify"]
  Verify --> Access["Allow or deny access"]
```

## Responsibilities

- Verify trust assertions.
- Gate access to protected capabilities.
- Remain compatible with security policy.

## Non-Responsibilities

- Choose a credential format.
- Define transport encryption.
- Conflate authentication with authorization.

## Notes

Authentication should be explicit and observable from a protocol perspective.

## References

- [permissions.md](permissions.md)
- [../12-security/security-model.md](../12-security/security-model.md)
- [../10-protocol/handshake.md](../10-protocol/handshake.md)

## Acceptance Criteria

- Authentication behavior is clear.
- The server trust boundary is explicit.
- The document avoids implementation coupling.
