<!--
engineering/languages/swift.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Swift Development Practices

Use the project's declared Swift toolchain and supported Apple platforms. Prefer concrete value
types for pure state, actors for mutable asynchronous state, and narrow protocols at framework,
persistence, or network boundaries that benefit from substitution. Avoid unnecessary protocols and
generics for simple calculations.

Group declarations by responsibility: nested types, stored properties, computed API, initializers,
methods, related static API, then private helpers. Enum cases generally precede
identity/display/query behavior. Alphabetical order may suit lookup tables; do not mechanically
alphabetize mixed API surfaces.

Order SwiftUI views as environment, inputs, state, body, extracted views, actions, and
formatting/private helpers. Keep views declarative and business rules testable. Use the project's
design tokens and accessible controls. Preserve DocC contracts, meaningful MARK sections, and
supported platform behavior.

Avoid force unwraps and unchecked production casts. Inject clocks, services, persistence, and
diagnostics where deterministic behavior matters. Keep privacy-sensitive data out of fixtures and
logs. For persisted models, preserve historical schemas and introduce explicit migrations.
CloudKit-compatible relationships and conflict behavior require project-specific tests and manual
device evidence.

Use the [Swift instructions template](../templates/copilot/swift.instructions.md) and
[testing template](../templates/copilot/swift-testing.instructions.md), installing project-specific globs locally.
