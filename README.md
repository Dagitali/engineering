<!--
engineering/README.md
Dagitali organization documentation

Responsibilities
- Index shared engineering guidance and clarify adoption boundaries.

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
- [Contributing](#contributing)
- [Validation and Scope](#validation-and-scope)

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

## Contributing

Read the [contributor guide] and [repository instructions] before editing. Keep reusable guidance
separate from project-owned contracts, and keep source templates blank.

## Validation and Scope

Use the contributor guide's [validation procedure] for this checkout. Review local destinations,
heading anchors, reference labels, and template placeholders alongside source accuracy. Local checks
do not establish external availability, hosted enforcement, or publication. Browse the [runbook
index] for bounded operational procedures and the [playbook index] for change planning.

[repository instructions]: AGENTS.md
[contributor guide]: CONTRIBUTING.md
[validation procedure]: CONTRIBUTING.md#validation
[Source notices]: NOTICES.md
[Automation]: automation/README.md
[Development workflow]: development/agent-assisted-workflow.md
[Documentation maintenance]: documentation/maintenance.md
[Branch protection]: governance/branch-protection.md
[playbook index]: playbooks/README.md
[Change management]: playbooks/change-management.md
[runbook index]: runbooks/README.md
[Templates]: templates/README.md
