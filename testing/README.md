<!--
engineering/testing/README.md
Dagitali organization documentation

Responsibilities
- Index validation layers and operational evidence boundaries.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Testing Guidance

Choose tests by the changed boundary. The consuming project owns discovery, command names, tool
versions, fixtures, and its applicable quality gate.

- [Local Validation](#local-validation)
- [Operational Evidence](#operational-evidence)

## Local Validation

- [Python testing]: Deterministic tests, compatibility evidence, and clean artifact installation.
- [Infrastructure testing]: Synthesis, property assertions, and resource-change review.
- [Automation contracts]: Workflow/action interfaces, fixtures, and evidence limits.

## Operational Evidence

Use [disposable cloud tests] only within an authorized bounded scope. Keep deployed, device, hosted,
and publication evidence distinct from local checks. Use [release evidence] for candidate identity
and recorded outcomes, and [runbooks] for diagnosis and recovery.

[release evidence]: ../releases/evidence-and-history.md
[runbooks]: ../runbooks/README.md
[Automation contracts]: automation-contracts.md
[disposable cloud tests]: disposable-cloud-tests.md
[Infrastructure testing]: infrastructure.md
[Python testing]: python.md
