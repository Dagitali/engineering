<!--
engineering/README.md
Dagitali organization documentation

Maintainer Notes
- Keep shared guidance independent of any originating project.
-->

# Dagitali Engineering

Shared development practices, review procedures, and reusable documentation templates for Dagitali
projects. Each project retains its own executable configuration, licensing, support commitments,
release policy, and hosted settings.

- [Start Here](#start-here)
- [Adoption](#adoption)
- [Topic Guides](#topic-guides)

## Start Here

- [Development workflow]
- [Documentation maintenance]
- [Change management]
- [Branch protection]
- [Automation]
- [Templates]
- [Source notices]

## Adoption

Use shared guidance alongside the project's local instructions. Replace template fields before
installing a template in a consuming repository. Local commands, supported versions, branch routes,
permissions, and product guarantees remain authoritative in that project.

This repository contains reusable practice and blank templates. Project catalogs, migration
inventories, completed operational records, and product-specific contracts belong to their owners.
Read the [retained notices][Source notices] for applicable material terms; hosting does not
establish a new license.

## Topic Guides

- [Python](languages/python.md) and [Swift](languages/swift.md)
- [Python testing](testing/python.md), [infrastructure testing](testing/infrastructure.md),
  and [disposable cloud tests](testing/disposable-cloud-tests.md)
- [Interface evolution](interfaces/evolution-checklist.md)
- [Architecture decisions](architecture/decision-records.md)
- [GitFlow option](git/gitflow.md)
- [Ownership and exceptions](governance/ownership-and-exceptions.md)
- [Release evidence](releases/evidence-and-history.md), [Python releases](releases/python-packages.md),
  [Apple app releases](releases/apple-apps.md), and [shared automation releases](releases/shared-automation.md)
- [Repository incident response](runbooks/repository-ci-incident.md),
  [required check transitions](runbooks/update-required-checks.md),
  [hosted settings audits](runbooks/hosted-settings-audit.md), and
  [shared automation incidents](runbooks/shared-automation-incident.md)
- [Automation contract testing](testing/automation-contracts.md)
- [Workflow trust boundaries](security/workflow-trust-boundaries.md)
- [CDK change safety](infrastructure/cdk-change-safety.md)
- [Tooling lessons](learnings/python-and-repository-tooling.md)

[Source notices]: NOTICES.md
