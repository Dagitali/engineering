<!--
engineering/testing/automation-contracts.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide deterministic workflow and action interface validation.

Responsibilities
- Guide deterministic workflow and action interface validation.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Automation Contract Testing

- [Contract Scope](#contract-scope)
- [Fixtures and Evidence Boundaries](#fixtures-and-evidence-boundaries)

## Contract Scope

Test workflow/action interfaces alongside their documentation: input types/defaults/forwarding,
commands, outputs, required permissions, runner/layout assumptions, artifacts, cancellation, and
emitted checks. Retain parity tests when workflows and composite actions share validation behavior.

## Fixtures and Evidence Boundaries

Use deterministic fixtures without credentials. Validate syntax/pins and actual command behavior;
log relevant tool versions. Fixtures must remain self-contained when copied into consumer checkouts.
Manual candidate matrices and representative hosted callers establish separate runtime evidence.
Neither local lint nor fixture success proves access policy, merge-queue blocking, publication, or
rollout.

Keep actual fixture paths, runtime combinations, commands, and public interfaces in the automation
library.
