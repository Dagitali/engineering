<!--
engineering/runbooks/README.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Index bounded operational checks and incident recovery procedures.

Responsibilities
- Index bounded operational checks and incident recovery procedures.

Maintainer Notes
- Keep concrete commands and confidential records with their owners.
-->

# Engineering Runbooks

Choose a procedure for the observed operational problem. Consuming projects own concrete commands,
access, recovery decisions, and completed records.

- [Repository and CI incidents]: Diagnose failing checks and validate recovery at the exact
  revision.
- [Shared automation incidents]: Assess affected revisions, containment, migration, and disclosure.
- [Hosted settings audits]: Compare read-only observations with explicit expectations.
- [Required-check transitions]: Coordinate replacement checks and verify hosted blocking behavior.

Use the [branch protection guide] for policy and the [playbook index] for broader change planning.
Keep sensitive evidence in restricted storage. Procedures do not independently authorize hosted
writes, credential changes, deployment, or publication.

[branch protection guide]: ../governance/branch-protection.md
[playbook index]: ../playbooks/README.md
[Hosted settings audits]: hosted-settings-audit.md
[Repository and CI incidents]: repository-ci-incident.md
[Shared automation incidents]: shared-automation-incident.md
[Required-check transitions]: update-required-checks.md
