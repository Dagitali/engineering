<!--
engineering/playbooks/change-management.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide compatibility decisions and synchronized validation and release.

Responsibilities
- Guide compatibility decisions and synchronized validation and release.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Change Management

Take a bounded requirement through implementation, review, and verified handoff. Choose evidence by
the changed boundary, preserving each project's contracts and review policy.

- [Classify the Change](#classify-the-change)
- [Define Supported Behavior](#define-supported-behavior)
- [Synchronize and Release](#synchronize-and-release)

## Classify the Change

| Boundary | Review | Evidence |
| --- | --- | --- |
| Public interface | Inputs, defaults, outputs, errors, compatibility | Positive, negative, boundary, and integration tests |
| Persistent data or infrastructure | Ownership, replacement, migration, retention, privacy, cost | Migration/synthesis tests and authorized operational review |
| Packaging | Metadata, dependencies, artifacts, installed entry points | Artifact inspection and clean installation |
| Delivery | Triggers, permissions, identity, checks, rollback | Contract checks and separate hosted evidence |
| Documentation | Canonical claims, navigation, attribution | Source review, links, relevant builds |

A change spanning boundaries needs evidence for each affected boundary.

## Define Supported Behavior

Before adding a component, state its demonstrated need, single responsibility, owner, entry point,
supported configuration, failure behavior, tests, and rollback. Avoid speculative APIs and
placeholder services. Keep reusable components separate from consumer identity, account
configuration, content, monitoring, budgets, and product-specific policy.

## Synchronize and Release

Use the [interface checklist], project impact map, and [documentation maintenance]. Update changed
claims during implementation. Record material alternatives in an architecture decision and reusable
diagnosed failures in a runbook.

Use the project's release procedure to assess the complete diff, compatibility, migration, artifact
identity, and recovery. Report local checks, hosted checks, and publication as separate outcomes.

[documentation maintenance]: ../documentation/maintenance.md
[interface checklist]: ../interfaces/evolution-checklist.md
