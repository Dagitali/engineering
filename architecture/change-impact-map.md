<!--
engineering/architecture/change-impact-map.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Source and validation ownership for changes to this documentation collection.

Responsibilities
- Identify the smallest complete documentation review scope.

Maintainer Notes
- Preserve canonical paths, blank templates, and historical evidence.
-->

# Change Impact Map

Use this map for changes to this collection. Consumers use the blank [impact template] with their
own sources and commands. This map identifies review scope rather than imposing a repository layout.

- [Changed Surfaces](#changed-surfaces)
- [Review Lenses](#review-lenses)
- [Boundary Rules](#boundary-rules)

## Changed Surfaces

| Changed surface | Canonical evidence | Related documents | Verification |
| --- | --- | --- | --- |
| Guidance or examples | Owning implementation or policy | Topic guides, indexes, references | Source accuracy, destinations, anchors |
| Template fields or instructions | Blank template and consumer requirements | Template index, adoption guides | Placeholders, copied paths, compatibility |
| Local setup or hooks | `.pre-commit-config.yaml` | Contributor guide, onboarding, security | Configuration, actual commands, side effects |
| Licensing or attribution | `LICENSE`, `NOTICE`, applicable source notices | README, contribution terms, notices | Authority, retained attribution, scope |
| Support or reporting | Owner-approved policy and available channels | Support, security, conduct, README | Accurate commitments and private routing |
| Version or release state | Candidate tree, tags, dated observations | Changelog, archive, version record | Identity, date basis, validation evidence |

Changes spanning rows need all applicable evidence. Follow the [validation procedure] and use the
[maintenance guide] to find other references to changed claims.

## Review Lenses

Review linked paths and headings, reference definitions, template replacement fields, source
accuracy, attribution, and adoption effects. Distinguish reusable advice from this checkout’s own
policy. Preserve language- and platform-specific detail where it serves a real contract.

Use the [interface checklist] for changes that affect accepted inputs or consumer behavior. Keep
current policy separate from historical tagged records and explain migrations without silently
rewriting adopted copies.

## Boundary Rules

Keep templates blank and private completed records outside this checkout. Documentation edits do not
establish hosted enforcement or authorize operational changes. Preserve unrelated work and immutable
tags. Use the [release playbook] for separately authorized release preparation and delivery.

[validation procedure]: ../CONTRIBUTING.md#validation
[maintenance guide]: ../documentation/maintenance.md
[interface checklist]: ../interfaces/evolution-checklist.md
[release playbook]: ../playbooks/release.md
[impact template]: ../templates/change-impact-map.md
