<!--
engineering/automation/validation-and-delivery.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Separate consumer validation from authorized delivery operations.

Responsibilities
- Separate consumer validation from authorized delivery operations.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Validation and Delivery

- [Validation Scope](#validation-scope)
- [Workflow Responsibilities](#workflow-responsibilities)
- [Caller Adoption](#caller-adoption)
- [Delivery and Recovery](#delivery-and-recovery)

## Validation Scope

Keep ordinary validation separate from deployment, package publication, signing, and hosted
administration. Shared workflows validate a consumer; they do not assume its release identity or
control its infrastructure.

## Workflow Responsibilities

Document the actual workflow map in the owning project. Separate responsibilities even when a
project combines them into one workflow; this table does not require a particular file layout.

| Responsibility | Evidence to document | Boundary |
| --- | --- | --- |
| PR routing and review gates | Events, target branches, emitted results | Local declarations versus hosted enforcement |
| Source validation | Commands, fixtures, tool versions, failure behavior | Source results versus distributed behavior |
| Artifact validation | Build identity, contents, clean installation | Tested artifacts versus another build |
| Security and inventory | Audit scope, dependencies, SBOM inputs | Findings versus certification |
| Publication or deployment | Identity, approval, exact candidate, recovery | Validation versus authorized delivery |

For each applicable responsibility, record triggers, conditions, permissions, dependencies,
concurrency, result names, artifacts, and retention. Explain how downstream jobs receive the same
validated candidate and how skipped or failed upstream jobs affect delivery. Keep secrets out of
routine validation and grant write permissions only to jobs that require authorized writes.

This checkout’s hooks are documented in the [contributor guide]. They are local checks, not evidence
of consumer CI execution. Use the [required-check runbook] for coordinated hosted transitions.

## Caller Adoption

Choose caller events, cancellation, directories, commands, and required results for the actual
project. Verify caller behavior at an immutable revision. Copied starter files require independent
review when their contents change; updating a shared reference alone does not update copied
configuration.

## Delivery and Recovery

Delivery uses the project's reviewed workflow, explicit identity, environment controls, candidate
artifact, and rollback procedure. Local/source validation does not establish deployed compatibility
or signed binary behavior. Record each outcome separately and keep credentials out of routine
fixture tests.

[contributor guide]: ../CONTRIBUTING.md#local-setup-and-hooks
[required-check runbook]: ../runbooks/update-required-checks.md
