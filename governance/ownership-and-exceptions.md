<!--
engineering/governance/ownership-and-exceptions.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Explain ownership, exception records, and inactive-consumer review.

Responsibilities
- Explain ownership, exception records, and inactive-consumer review.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Ownership and Exceptions

- [Ownership Boundaries](#ownership-boundaries)
- [Override and Exception Records](#override-and-exception-records)
- [Review and Closure](#review-and-closure)
- [Inactive Consumers](#inactive-consumers)
- [Deprecated Shared Interfaces](#deprecated-shared-interfaces)

## Ownership Boundaries

Projects own their configuration, callers, licenses, support commitments, CODEOWNERS, and hosted
settings. Shared-library maintainers own released interfaces and their documentation. An override is
not automatically an error: preserve intentional consumer differences and document their impact.

## Override and Exception Records

For a policy exception or local override, record the affected surface, baseline revision,
alternative, reason, security/compatibility impact, compensating measures, responsible owner,
applicable approval, decision date, next review, evidence, and removal or migration condition.
Choose review intervals by risk; this guidance establishes no universal deadline or central approval
service.

## Review and Closure

Recheck after ownership, visibility, workflow, or policy changes. Close superseded records with the
replacement decision and retain useful history. Hosted owner access and bypass behavior require
separate verification. Completed records with private details belong in restricted storage.

## Inactive Consumers

For inactive consumers, record maintenance status, owner availability, adopted revision, outstanding
findings, and disclosure/update expectations. Inactivity does not authorize disabling workflows,
archiving repositories, or deleting evidence. Track known migrations separately from unknown
adoption. Use the [inventory template] and the component's local release policy.

## Deprecated Shared Interfaces

Follow the component's local release policy when deprecating an interface. Announce the affected
paths, inputs, or behavior, identify a replacement where feasible, and document migration steps.
Retain released revisions and distinguish known consumer migrations from unknown adoption; missing
inventory is not evidence that an interface is unused.

Assign each known migration an owner, target revision, validation evidence, and reviewed recovery
reference. Removal requires the component's versioning decision and compatibility review. Updating a
starter does not update previously copied callers. Retain dated migration or retirement decisions
without silently rewriting consumers or retargeting immutable tags. Use the [interface checklist]
and [shared automation release guide] where applicable.

[interface checklist]: ../interfaces/evolution-checklist.md
[shared automation release guide]: ../releases/shared-automation.md
[inventory template]: ../templates/consumer-inventory.md
