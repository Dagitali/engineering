<!--
engineering/ARCHITECTURE.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Repository structure, adoption flow, and ownership boundaries.

Responsibilities
- Explain architecture and its ownership boundaries.

Maintainer Notes
- Link canonical guidance and preserve purposeful project differences.
-->

# Architecture

- [System Context](#system-context)
- [Repository Architecture](#repository-architecture)
- [Adoption Flow](#adoption-flow)
- [Trust Boundaries](#trust-boundaries)
- [Change Impact and Sources of Truth](#change-impact-and-sources-of-truth)

## System Context

This repository supplies shared engineering guidance and blank templates. Consumers select and adapt
them alongside their own implementation and policy. It has no application runtime or deployment
service. The [repository overview] is the entry point.

## Repository Architecture

| Area | Responsibility |
| --- | --- |
| Root policies | Contribution, licensing, support, security, and this repository’s releases |
| Topic guides | Reusable development, testing, governance, and operational practices |
| [Templates] | Blank project-owned planning and verification forms |
| [Documentation guidance] | Source accuracy, navigation, and maintenance |
| [Release archive] | Historical records for this repository |
| Local hook configuration | Optional checks and formatting tools described in [contribution guidance] |

## Adoption Flow

1. Identify a demonstrated consumer requirement and its local owner.
2. Select a reviewed source revision and only the relevant guidance or templates.
3. Adapt paths, fields, commands, and policy to the consumer.
4. Validate the changed boundary and record the adopted revision.
5. Review later updates against local adaptations using the [adoption playbook].

## Trust Boundaries

Consumers own execution, credentials, hosted settings, and product contracts. Hooks can execute
tools and rewrite files; review their configuration before running them. Documentation validation
does not establish hosted enforcement or deployed behavior. See the [security policy].

## Change Impact and Sources of Truth

Use this collection’s [change impact map] for local edits and the blank [impact template] for
consumer-owned contracts, sources, checks, documentation, and owners. Keep component architecture
and completed maps with their implementations. The [maintenance guide] owns source review; [design
guidance] explains reusable-content constraints.

[contribution guidance]: CONTRIBUTING.md#local-setup-and-hooks
[design guidance]: DESIGN.md
[repository overview]: README.md
[security policy]: SECURITY.md
[change impact map]: architecture/change-impact-map.md
[Documentation guidance]: documentation/README.md
[maintenance guide]: documentation/maintenance.md
[adoption playbook]: playbooks/adopt-shared-guidance.md
[Release archive]: releases/history/README.md
[Templates]: templates/README.md
[impact template]: templates/change-impact-map.md
