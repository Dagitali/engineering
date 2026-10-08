<!--
engineering/testing/dependency-consistency.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Dependency declaration, lockfile, and installation evidence boundaries.

Responsibilities
- Guide consistency review without prescribing a package manager.

Maintainer Notes
- Keep supported formats and resolution rules owned by the selected tool.
-->

# Dependency Consistency

Review dependency declarations and resolved state using the project’s own package manager and
supported formats. A static comparison does not replace resolution, installation, or runtime tests.

- [Identify Authoritative Inputs](#identify-authoritative-inputs)
- [Compare Declared and Resolved State](#compare-declared-and-resolved-state)
- [Verify Installation and Behavior](#verify-installation-and-behavior)
- [Record Limitations and Recovery](#record-limitations-and-recovery)

## Identify Authoritative Inputs

Identify maintained manifests, committed locks, workspace boundaries, generated inputs, and any
source manifest copied by automation. Inspect what the actual build or installation consumes rather
than assuming the nearest manifest is authoritative. Record the package-manager version and update
procedure with the project.

## Compare Declared and Resolved State

Check applicable package identity, versions, dependency groups, and intended constraints. Keep
minimum-supported dependency fixtures aligned with declared support, while preserving neutral
fixtures that test arbitrary consumer policy. A fixture change alone need not authorize dropping
support for older dependencies.

Respect format-specific resolution rules. Static root comparisons can miss transitive dependencies,
peer relationships, workspaces, platform-specific choices, and range resolution. Document exactly
which relationships a selected validator covers; retain checks for uncovered requirements.

## Verify Installation and Behavior

Use the project’s reproducible installation procedure in an isolated environment, then run the
relevant behavior checks. Preserve frozen or locked installation semantics where promised. Record
network, credential, and filesystem boundaries before execution; installation may execute package
code. Do not regenerate a lock merely to hide an unexplained mismatch.

Use [Python testing] for Python dependency-boundary and clean-artifact evidence. Use [automation
contracts] when CI copies or transforms manifests, and verify the generated inputs consumed by the
actual caller. Local consistency does not establish hosted installation or deployed behavior.

## Record Limitations and Recovery

Record the authoritative inputs, tool revision, commands, findings, skipped checks, and last
known-good configuration. Separate intentional dependency updates from tooling migration. Use
reviewed corrections or restore compatible inputs together; keep consumer-specific records and
sensitive diagnostics with their owner.

[automation contracts]: automation-contracts.md
[Python testing]: python.md
