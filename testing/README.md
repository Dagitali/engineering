<!--
engineering/testing/README.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Index validation layers and operational evidence boundaries.

Responsibilities
- Index validation layers and operational evidence boundaries.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Testing Guidance

Choose tests by the changed boundary. The consuming project owns discovery, command names, tool
versions, fixtures, and its applicable quality gate.

- [Local Validation](#local-validation)
- [Test Layers](#test-layers)
- [Dependency Boundaries](#dependency-boundaries)
- [Operational Evidence](#operational-evidence)

## Local Validation

For each changed boundary, identify its contract and select positive, negative, and boundary
evidence where useful. Run focused checks first, then the project’s applicable broader gate. Keep
fixtures deterministic and sanitized; do not introduce credentials or external operations merely to
exercise a local contract. Record skipped checks and limitations alongside results.


- [Python testing]: Deterministic tests, compatibility evidence, and clean artifact installation.
- [Infrastructure testing]: Synthesis, property assertions, and resource-change review.
- [Automation contracts]: Workflow/action interfaces, fixtures, and evidence limits.

## Test Layers

| Layer | Evidence | Boundary to review |
| --- | --- | --- |
| Static and documentation checks | Formats, destinations, declared contracts | Parser coverage and source accuracy |
| Unit and integration tests | Isolated behavior and composed entry points | Fixtures, discovery, and environment |
| Artifact and installation checks | Distributed contents and behavior outside the source checkout | Build identity, clean environments, package-index access |
| Device or deployed tests | Actual runtime behavior | Signing, accounts, resources, privacy, and cleanup |
| Hosted checks | Workflow results and enforcement | Access, required results, and dated observations |

Select only applicable layers. A passing layer does not substitute for evidence at another boundary.
Command names and test discovery remain project-owned; report which layers actually ran.

## Dependency Boundaries

Use [dependency consistency] to review manifests, locks, generated inputs, and installation evidence.

Document tool installation separately from test execution. Identify network, credentials, writable
paths, subprocesses, and resource creation before running a check. Use isolated environments for
supported dependency ranges and verify that fixture pins match declared contracts. Keep ordinary
local fixtures independent of live services where feasible. See [Python testing] for
language-specific dependency and artifact guidance.

## Operational Evidence

Use [disposable cloud tests] only within an authorized bounded scope. Keep deployed, device, hosted,
and publication evidence distinct from local checks. Use [release evidence] for candidate identity
and recorded outcomes, and [runbooks] for diagnosis and recovery.

[release evidence]: ../releases/evidence-and-history.md
[runbooks]: ../runbooks/README.md
[Automation contracts]: automation-contracts.md
[dependency consistency]: dependency-consistency.md
[disposable cloud tests]: disposable-cloud-tests.md
[Infrastructure testing]: infrastructure.md
[Python testing]: python.md
