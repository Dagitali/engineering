---
applyTo: "**/*Tests/**/*.swift,**/*UITests/**/*.swift"
---
<!--
engineering/templates/copilot/swift-testing.instructions.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Provide adaptable Swift testing and evidence instructions.

Responsibilities
- Provide adaptable Swift testing and evidence instructions.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Swift Testing Instructions Template

Install locally with `applyTo: "<unit paths>,<integration paths>,<UI paths>,<repository test
paths>"`.

- Use Swift Testing for supported unit/integration/repository tests and XCTest/XCUITest where UI
  automation requires it.
- Name behavior clearly and parameterize concise cases.
- Inject clocks, services, persistence writers, and settings; avoid wall-time/network/global-state
  dependencies.
- Use in-memory persistence for isolated tests and explicit disk fixtures for migration behavior.
- Exercise relevant success, failure, retry, cancellation, deduplication, migration, privacy, and
  relationships.
- Drive UI tests through accessibility identifiers and observable state; fix races instead of adding
  fixed sleeps.
- Keep host-side repository inspection in `<designated unsandboxed test package>` when required by
  the project.
- Keep fixtures, attachments, diagnostics, and messages free of private user data.

Use actual project suite paths, platform scope, and validation commands rather than these fields.
