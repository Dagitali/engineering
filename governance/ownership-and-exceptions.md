<!--
engineering/governance/ownership-and-exceptions.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Ownership and Exceptions

Projects own their configuration, callers, licenses, support commitments, CODEOWNERS, and hosted
settings. Shared-library maintainers own released interfaces and their documentation. An override is
not automatically an error: preserve intentional consumer differences and document their impact.

For a policy exception or local override, record the affected surface, baseline revision,
alternative, reason, security/compatibility impact, compensating measures, responsible owner,
applicable approval, decision date, next review, evidence, and removal or migration condition.
Choose review intervals by risk; this guidance establishes no universal deadline or central approval
service.

Recheck after ownership, visibility, workflow, or policy changes. Close superseded records with the
replacement decision and retain useful history. Hosted owner access and bypass behavior require
separate verification. Completed records with private details belong in restricted storage.

For inactive consumers, record maintenance status, owner availability, adopted revision, outstanding
findings, and disclosure/update expectations. Inactivity does not authorize disabling workflows,
archiving repositories, or deleting evidence. Track known migrations separately from unknown
adoption. Use the [inventory template](../templates/consumer-inventory.md) and the component's local
release policy.
