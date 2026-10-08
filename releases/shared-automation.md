<!--
engineering/releases/shared-automation.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Guide interface versioning and verified consumer adoption.

Responsibilities
- Guide interface versioning and verified consumer adoption.

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Shared Automation Releases

- [Compatibility and Interface Scope](#compatibility-and-interface-scope)
- [Candidate Validation](#candidate-validation)
- [Publication and Consumer Rollout](#publication-and-consumer-rollout)

## Compatibility and Interface Scope

Version workflow/action paths, inputs, types, defaults, outputs, runner requirements, permissions,
and artifact contracts as public interfaces. Assess compatibility by consumer impact, including
changed defaults or required permissions, rather than file count.

## Candidate Validation

Validate local contracts and representative hosted callers at the candidate revision. Record exact
tool, runner, command, artifact, access, merge-group, and cancellation evidence. Distinguish
configurable but unverified combinations from tested support. Use the [automation release template].

## Publication and Consumer Rollout

Consumers should select existing reviewed immutable revisions. Moving major tags are optional
maintained release lines; do not invent them or retarget immutable tags. Replacing a shared revision
and updating copied starters require separate review. Stage rollout to known consumers, retain the
prior known-good reference, and record unknown adoption. Publishing the shared library neither
publishes consumer packages nor deploys consumer infrastructure.

[automation release template]: ../templates/releases/shared-automation.md
