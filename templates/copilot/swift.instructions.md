---
applyTo: "**/*.swift"
---
<!--
engineering/templates/copilot/swift.instructions.md
Dagitali organization documentation

Responsibilities
- Provide adaptable Swift source and documentation instructions.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Swift Source Instructions Template

Install locally with `applyTo: "<source directories>/**/*.swift"`; choose actual project paths and
toolchain.

- Prefer values for pure state, actors for mutable asynchronous state, and narrow protocols at
  service boundaries.
- Avoid unnecessary abstractions, production force unwraps, and unchecked casts.
- Keep SwiftUI declarative; move business rules to testable models/services and use local design
  tokens.
- Preserve supported platforms, stable accessibility identifiers, DocC contracts, and meaningful
  MARK structure.
- Order views as environment, inputs, state, body, extracted views, actions, and helpers.
- Preserve frozen persisted schemas and introduce explicit migration stages for model changes.
- Use CloudKit-compatible relationships where needed and test conflicts/deduplication rather than
  assuming immediate sync.
- Inject privacy-safe diagnostics, clocks, persistence, and framework/network services where
  substitution matters.

`<Add local capture/permission/data-retention and platform rules; do not copy another app's privacy promises>`.
