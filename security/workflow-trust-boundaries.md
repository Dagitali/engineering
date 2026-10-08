<!--
engineering/security/workflow-trust-boundaries.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide workflow identity, privilege, and untrusted-code review.

Responsibilities
- Guide workflow identity, privilege, and untrusted-code review.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Workflow Trust Boundaries

- [Event and Code Trust](#event-and-code-trust)
- [Permissions and Identity](#permissions-and-identity)
- [Validation Boundaries](#validation-boundaries)

## Event and Code Trust

Review each workflow by event, checked-out code, commands executed, identity, permissions, secrets,
environments, artifacts, and downstream consumers. Pin remote actions to reviewed full commit SHAs;
a pin provides reproducibility, not proof that referenced code is safe.

Privileged events such as `pull_request_target` and `workflow_run` need an explicit trust analysis.
Do not execute untrusted contribution code with privileged credentials. Keep exceptions narrow,
owned, reviewed, and time-bounded where the project's policy requires expiry. Repository
configuration establishes expected policy, not hosted enforcement.

Do not interpolate untrusted event data directly into shell command text. Pass it as data through an
environment variable or a structured input, quote expansions, and validate it before use. These
steps do not make executing the supplied value as a command safe. Review the complete path from
event input to checkout, command execution, artifacts, and downstream privileged jobs.

## Permissions and Identity

Use job-scoped least privilege and keep ordinary validation credential-free. Command inputs, builds,
and synthesis execute trusted project code; they are not sandbox boundaries. Separate dependency
findings, inventory, and security assurance: an SBOM is not a vulnerability verdict or
certification.

## Validation Boundaries

Use [dependency consistency] when reviewing manifest and lockfile pairs; static agreement does not
prove full dependency resolution or safe installation.

The chosen validator's reference owns its configuration schema and limitations. Keep actual workflow
selection, applicable manifest/lock pairs, exceptions, and installed tool revision in the consuming
project.

[dependency consistency]: ../testing/dependency-consistency.md
