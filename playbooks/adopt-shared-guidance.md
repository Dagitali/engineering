<!--
engineering/playbooks/adopt-shared-guidance.md
Dagitali organization documentation

Copyright © 2026 Dagitali LLC. All rights reserved.

Explain adopt shared guidance and its ownership boundaries.

Responsibilities
- Explain adopt shared guidance and its ownership boundaries.

Maintainer Notes
- Link canonical guidance and preserve purposeful project differences.
-->

# Adopt Shared Guidance

- [Choose the Adoption Path](#choose-the-adoption-path)
- [Prepare the Consumer](#prepare-the-consumer)
- [Capture the Existing Baseline](#capture-the-existing-baseline)
- [Integrate and Validate](#integrate-and-validate)
- [Retain Migration Safeguards](#retain-migration-safeguards)
- [Feed Evidence Back](#feed-evidence-back)

## Choose the Adoption Path

For a new project, use [consumer scaffolding]. For an existing project, treat replacing guidance,
templates, or validators as a migration. Select the smallest useful scope; adopting one guide does
not require copying this repository’s layout, tools, or branch model.

## Prepare the Consumer

Identify the owner, local instructions, contracts, toolchain, and review route. Choose a reviewed
source commit or tag and inspect its applicable license and notices. Use [templates] only after
replacing fields and checking paths. Keep completed records with the consumer.

## Capture the Existing Baseline

Record current instructions, callers, commands, exclusions, expected results, and required checks.
For validator replacement, compare known-good, failing, and boundary fixtures using [policy-check
guidance]. Classify differences as intentional local policy, unsupported behavior, or defects.

## Integrate and Validate

Preserve local contracts and coverage during comparison. Verify copied commands, links, installed
instruction paths, and actual behavior before retiring an existing procedure. Run the consumer’s
applicable gate. Use the [required-check runbook] for separately authorized hosted transitions.

## Retain Migration Safeguards

Record the prior revision, adopted source, local adaptations, validation, owner, and recovery path.
Use [template update guidance] for later changes. Restore compatible behavior through reviewed
corrections rather than silently weakening checks or moving tags.

## Feed Evidence Back

Report reusable requirements with minimal sanitized examples and expected behavior. Keep product
policy and private evidence local. Use the [interface checklist] to review shared-contract changes.

[policy-check guidance]: ../automation/repository-policy.md
[interface checklist]: ../interfaces/evolution-checklist.md
[required-check runbook]: ../runbooks/update-required-checks.md
[templates]: ../templates/README.md
[template update guidance]: ../templates/README.md#updating-adopted-templates
[consumer scaffolding]: scaffold-consumer-project.md
