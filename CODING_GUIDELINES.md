# Coding Guidelines

## Index

- [Intent](#intent)
- [General Rules](#general-rules)
- [Boundary Rules](#boundary-rules)
- [Documentation Rules](#documentation-rules)

## Intent

These guidelines exist to keep the codebase readable, predictable, and easy to evolve over time.
They are intentionally conservative because Resonance is being built for longevity.

## General Rules

- Prefer small modules with one responsibility.
- Favor explicit naming over clever abstractions.
- Keep public surfaces narrow and stable.
- Optimize for clarity before optimization.

## Boundary Rules

- Do not introduce engine dependencies into the core layer.
- Do not couple SDK concerns to server concerns.
- Keep protocol definitions independent from runtime transport decisions.

## Documentation Rules

- Update architecture and foundation documents when the shape of the project changes.
- Use ADRs for decisions with long-term consequences.
- Keep terminology consistent across all documentation.
