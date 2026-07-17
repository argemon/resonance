# SDK Architecture

## Index

- [Purpose](#purpose)
- [SDK Responsibilities](#sdk-responsibilities)
- [Language and Engine Separation](#language-and-engine-separation)

## Purpose

SDKs are the adaptation layer between Resonance concepts and specific runtime ecosystems.

## SDK Responsibilities

- Translate core concepts into engine-friendly APIs.
- Preserve core semantics while fitting local conventions.
- Keep language bindings and engine bindings modular.

## Language and Engine Separation

Language SDKs and engine SDKs may share design intent, but they should not be forced into a single implementation shape.
Each adapter should remain independently maintainable.
