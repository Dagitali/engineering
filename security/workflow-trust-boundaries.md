<!--
engineering/security/workflow-trust-boundaries.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Workflow Trust Boundaries

Review each workflow by event, checked-out code, commands executed, identity, permissions, secrets,
environments, artifacts, and downstream consumers. Pin remote actions to reviewed full commit SHAs;
a pin provides reproducibility, not proof that referenced code is safe.

Privileged events such as `pull_request_target` and `workflow_run` need an explicit trust analysis.
Do not execute untrusted contribution code with privileged credentials. Keep exceptions narrow, owned,
reviewed, and time-bounded where the project's policy requires expiry. Repository configuration establishes
expected policy, not hosted enforcement.

Use job-scoped least privilege and keep ordinary validation credential-free. Command inputs, builds,
and synthesis execute trusted project code; they are not sandbox boundaries. Separate dependency findings,
inventory, and security assurance: an SBOM is not a vulnerability verdict or certification.

The chosen validator's reference owns its configuration schema and limitations. Keep actual workflow selection, applicable manifest/lock pairs,
exceptions, and installed tool revision in the consuming project.
