<!--
engineering/templates/change-impact-map.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Blank change impact map for project-owned planning and verification.

Responsibilities
- Provide a blank change impact map template.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Change Impact Map Template

Populate with actual project paths and commands. Keep the completed map in the project; it describes
review scope, not another implementation specification.

## Changed Surfaces

| Changed surface | Canonical source | Tests | Focused validation | Maintained docs | Owner |
| --- | --- | --- | --- | --- | --- |
| Commands/interfaces | | | | | |
| Configuration/defaults | | | | | |
| Data/resources/trust | | | | | |
| Packaging/dependencies | | | | | |
| Workflows/checks/artifacts | | | | | |
| Release behavior | | | | | |

Changes spanning multiple rows require all applicable source, test, and documentation evidence.
Choose focused checks from the consuming project's command definitions, then run its applicable
broader gate. Record skipped or unavailable checks without treating them as successful.

## Review Lenses

Review compatibility, failure behavior, privacy, accessibility, migration, retention, permissions,
resource replacement, availability, and cost where applicable. Preserve intentional consumer
differences.

## Boundary Rules

Keep sources, commands, owners, and completed records in the consuming project. This map identifies
review scope; it does not establish new support promises or authorize implementation, deployment,
publication, or hosted changes. Preserve unrelated work and historical evidence, and report
discrepancies requiring a separate decision.
